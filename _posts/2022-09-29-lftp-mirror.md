layout: post
title: "Testing 123"
date: 2022-09-29 22:53:00 -0000
categories: learning-github-pages

# Using lftp to mirror data from an android phone. 
* Ensure the phone and computer are on the same wifi network.
* Start MixPlorer 
* Start FTP server on the phone.
* On the computer...
```
lftp Admin@192.168.0.143:2121
Password: 
lftp Admin@192.168.0.143:~> ls                    
...
```
* If the 'ls' works, then issue the mirror command. To mirror everything, use the below
** -c: continue
** --parallel=N no. of parallell downloads
```
mirror -c --parallel=10
```
 
