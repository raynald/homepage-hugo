+++
bref = ""
date = "2017-05-25T14:47:53+02:00"
description = "Some small tricks"
draft = false
title = "Tech"
toc = true
weight = 20

+++

### How to encrypt and decrypt a file

*Encrypt*:

> openssl aes-256-cbc -a -salt -in secrets.txt -out secrets.txt.enc

*Decrypt*:

> openssl aes-256-cbc -d -a -in secrets.txt.enc -out secrets.txt.new

### How to use bash to generate a random number
> $(( ( RANDOM % BUCKET )  + 1 ))

### How to fix Chinese font issue on Nook Simple Touch

Replace chinese fonts with following one.

```
@font-face {
font-family:"cnepub";
src:url(res:///opt/sony/ebook/FONT/tt0011m_.ttf), url(res:///tt0011m_.ttf),
   url(res:///ebook/fonts/../../mnt/sdcard/fonts/zw.ttf),
    url(res:///ebook/fonts/../../mnt/extsd/fonts/zw.ttf),
    url(res:///ebook/fonts/zw.ttf),
    url(res:///ebook/fonts/DroidSansFallback.ttf),   url(res:///fonts/ttf/zw.ttf),
   url(res:///../../media/mmcblk0p1/fonts/zw.ttf),   url(res:///DK_System/system/font/zw.ttf),   url(res:///abook/ fonts/zw.ttf),   url(res:///system/fonts/zw.ttf),
    url(res:///system/media/sdcard/fonts/zw.ttf),
    url(res:///media/fonts/zw.ttf),
    url(res:///sdcard/fonts/zw.ttf),
    url(res:///system/fonts/DroidSansFallback.ttf),url(res:///mnt/MOVIFAT/font/zw.ttf),url(fonts/zw.ttf);
}
```
