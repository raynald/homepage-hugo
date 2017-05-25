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


