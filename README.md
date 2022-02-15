## GDownloader    

Download Big files from google Drive with resumable link. The downlaoder function is taken from [here](https://askubuntu.com/questions/770753/how-to-download-large-google-drive-file-with-resume-support-in-ubuntu).   

Usage :    

```    
./GDownloader.sh <google_drive_file_id> <saved_file_name_with_extension>  
```    

The example of file_id in google drive url 

![](pic.png)  

Example 

``` 
$ ./GDownloader.sh 1nByw5vbPdb2T4ZP0nvLTRfmoIU4oqqCa metasploitable3.ova

--2022-02-15 22:30:56--  https://docs.google.com/uc?export=download&confirm=0Yxz&id=1nByw5vbPdb2T4ZP0nvLTRfmoIU4oqqCa
Resolving docs.google.com (docs.google.com)... 142.250.67.238, 2404:6800:4009:814::200e
Connecting to docs.google.com (docs.google.com)|142.250.67.238|:443... connected.
HTTP request sent, awaiting response... 302 Moved Temporarily
Location: https://doc-0g-c0-docs.googleusercontent.com/docs/securesc/o42igjeht4r6a0lfdefdoiu6n00809q8/shdurpvai7c5835m4ps7b3g5jg4432t7/1644944400000/08018216150024196802/01554654767505337015Z/1nByw5vbPdb2T4ZP0nvLTRfmoIU4oqqCa?e=download [following]
--2022-02-15 22:30:57--  https://doc-0g-c0-docs.googleusercontent.com/docs/securesc/o42igjeht4r6a0lfdefdoiu6n00809q8/shdurpvai7c5835m4ps7b3g5jg4432t7/1644944400000/08018216150024196802/01554654767505337015Z/1nByw5vbPdb2T4ZP0nvLTRfmoIU4oqqCa?e=download
Resolving doc-0g-c0-docs.googleusercontent.com (doc-0g-c0-docs.googleusercontent.com)... 142.250.192.1, 2404:6800:4009:827::2001
Connecting to doc-0g-c0-docs.googleusercontent.com (doc-0g-c0-docs.googleusercontent.com)|142.250.192.1|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://docs.google.com/nonceSigner?nonce=vng44fcpsbjue&continue=https://doc-0g-c0-docs.googleusercontent.com/docs/securesc/o42igjeht4r6a0lfdefdoiu6n00809q8/shdurpvai7c5835m4ps7b3g5jg4432t7/1644944400000/08018216150024196802/01554654767505337015Z/1nByw5vbPdb2T4ZP0nvLTRfmoIU4oqqCa?e%3Ddownload&hash=7i3th8m21c7ogpm3nond5jra2og915su [following]
--2022-02-15 22:30:58--  https://docs.google.com/nonceSigner?nonce=vng44fcpsbjue&continue=https://doc-0g-c0-docs.googleusercontent.com/docs/securesc/o42igjeht4r6a0lfdefdoiu6n00809q8/shdurpvai7c5835m4ps7b3g5jg4432t7/1644944400000/08018216150024196802/01554654767505337015Z/1nByw5vbPdb2T4ZP0nvLTRfmoIU4oqqCa?e%3Ddownload&hash=7i3th8m21c7ogpm3nond5jra2og915su
Connecting to docs.google.com (docs.google.com)|142.250.67.238|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://doc-0g-c0-docs.googleusercontent.com/docs/securesc/o42igjeht4r6a0lfdefdoiu6n00809q8/shdurpvai7c5835m4ps7b3g5jg4432t7/1644944400000/08018216150024196802/01554654767505337015Z/1nByw5vbPdb2T4ZP0nvLTRfmoIU4oqqCa?e=download&nonce=vng44fcpsbjue&user=01554654767505337015Z&hash=7m4k4b2rvjb8d8uvamj26bobao9fj9e0 [following]
--2022-02-15 22:30:58--  https://doc-0g-c0-docs.googleusercontent.com/docs/securesc/o42igjeht4r6a0lfdefdoiu6n00809q8/shdurpvai7c5835m4ps7b3g5jg4432t7/1644944400000/08018216150024196802/01554654767505337015Z/1nByw5vbPdb2T4ZP0nvLTRfmoIU4oqqCa?e=download&nonce=vng44fcpsbjue&user=01554654767505337015Z&hash=7m4k4b2rvjb8d8uvamj26bobao9fj9e0
Connecting to doc-0g-c0-docs.googleusercontent.com (doc-0g-c0-docs.googleusercontent.com)|142.250.192.1|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 7374820352 (6.9G) [application/x-virtualbox-ova]
Saving to: ‘metasploitable3.ova’

metasploitable3.ova         0%[               ]  33.77M  1.01MB/s    eta 2h 0m
```  
