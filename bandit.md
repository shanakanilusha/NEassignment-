####Level 0

* username = bandit0
* password = bandit0


####level 0 to Level 1

* username = bandit0
* password = bandit0

  ######Things we have to do and the results
  “cat” it and grab the password for level1

  ```
  bandit0@melinda:~$ ls
    readme

    bandit0@melinda:~$ cat readme 
    boJ9jbbUNNfktd78OOpsqOltutMc3MY1
    ```


####level 1 to Level 2

* username = bandit1
* password = boJ9jbbUNNfktd78OOpsqOltutMc3MY1

  ######Things we have to do and the results
  delimit the dash to read it

    ```
    bandit1@melinda:~$ ls
    bandit1@melinda:~$ cat ./\- 
    CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
    ```


####level 2 to Level 3

* username = bandit2
* password = CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

  ######Things we have to do and the results

   ``` 
   bandit2@melinda:~$ ls
    spaces in this filename


    bandit2@melinda:~$ cat ./spaces\ in\ this\ filename 
    UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
    ```
    
    
####level 3 to Level 4

* username = bandit3
* password = UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

  ######Things we have to do and the results
```
bandit3@melinda:~$ ls
inhere
bandit3@melinda:~$ cd inhere
bandit3@melinda:~/inhere$ ls -la
total 12
drwxr-xr-x 2 root    root    4096 Nov 14  2014 .
drwxr-xr-x 3 root    root    4096 Nov 14  2014 ..
-rw-r----- 1 bandit4 bandit3   33 Nov 14  2014 .hidden
bandit3@melinda:~/inhere$ cat .hidden
pIwrPrtPN36QITSp3EQaw936yaFoFgAB
```
    
    
    

####level 4 to Level 5

* username = bandit4
* password = pIwrPrtPN36QITSp3EQaw936yaFoFgAB

  ######Things we have to do and the results
  password is somewhere in the inhere directory and is the only human readable file in the directory
   
   ```
bandit4@melinda:~$ ls
inhere
bandit4@melinda:~$ cd inhere
bandit4@melinda:~/inhere$ ls -la
total 48
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file00
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file01
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file02
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file03
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file04
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file05
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file06
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file07
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file08
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file09
drwxr-xr-x 2 root    root    4096 Nov 14  2014 .
drwxr-xr-x 3 root    root    4096 Nov 14  2014 ..
bandit4@melinda:~/inhere$ file ./-*
./-file00: data
./-file01: data
./-file02: data
./-file03: data
./-file04: data
./-file05: data
./-file06: data
./-file07: ASCII text
./-file08: data
./-file09: data
bandit4@melinda:~/inhere$ cat ./-file07
koReBOKuIDDepwhWk7jZC0RTdopnAYKh
```
  

####level 5 to Level 6

* username = bandit5
* password = koReBOKuIDDepwhWk7jZC0RTdopnAYKh

  ######Things we have to do and the results
  similar to the level 4 to level 5
  
```  
bandit5@melinda:~$ ls 
inhere
bandit5@melinda:~$ cd inhere
bandit5@melinda:~/inhere$ ls -la
total 88
drwxr-x--- 22 root bandit5 4096 Nov 14  2014 .
drwxr-xr-x  3 root root    4096 Nov 14  2014 ..
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere00
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere01
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere02
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere03
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere04
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere05
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere06
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere07
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere08
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere09
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere10
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere11
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere12
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere13
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere14
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere15
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere16
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere17
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere18
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere19
bandit5@melinda:~/inhere$ find ./ -size 1033c
./maybehere07/.file2
bandit5@melinda:~/inhere$ cat ./maybehere07/.file2
DXjZPULLxYr17uwoI01bNLQbtFemEgo7
```

####level 6 to Level 7

* username = bandit6
* password = DXjZPULLxYr17uwoI01bNLQbtFemEgo7

  ######Things we have to do and the results
```
bandit6@melinda:~$ find / -user bandit7 -group bandit6 -size 33c 2>&1 | grep -v -F Permission
    /var/lib/dpkg/info/bandit7.password

    bandit6@melinda:~$ cat /var/lib/dpkg/info/bandit7.password
    HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
```  
    
####level 7 to Level 8

* username = bandit7
* password = HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

  ######Things we have to do and the results
  password for the next level is stored in the file data.txt
  
```  
 bandit7@melinda:~$ ls
    data.txt

    bandit7@melinda:~$ grep millionth data.txt
    millionth cvX2JJa4CFALtqS87jk27qwqGhBM9plV
```
    
####level 8 to Level 9

* username = bandit8
* password = cvX2JJa4CFALtqS87jk27qwqGhBM9plV

  ######Things we have to do and the results
  we need to find a unique line among many, so we have to pipe so commands
  
```
    bandit8@melinda:~$ ls
    data.txt

    bandit8@melinda:~$ sort data.txt | uniq --count | grep "1 "
    1 UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
```
    
    
####level 9 to Level 10

* username = bandit9
* password = UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

  ######Things we have to do and the results
  The password for the next level is stored in the file called data.txt among of few lines of human-readable strings starting with ‘=’ characters
  
```  
    bandit9@melinda:~$ ls
    data.txt
    bandit9@melinda:~$ strings data.txt | grep "="
    Rj=G
    ========== the
    =qy9g
    ,========== passwordc
    ========== is
    =9-5
    O=p~
    #r=t!
    7e}=eG
    ========== truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
    uXI/{I=VPO=
    6'Q|_=Vt
    :={!
    yd=6
``` 
    
####level 10 to Level 11

* username = bandit10
* password = truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk

  ######Things we have to do and the results
  passwordis stored in the file data.txt, which contains base64 encoded data, so we need to decord this file

```  
    bandit10@melinda:~$ ls
    data.txt
    bandit10@melinda:~$ cat data.txt
    VGhlIHBhc3N3b3JkIGlzIElGdWt3S0dzRlc4TU9xM0lSRnFyeEUxaHhUTkViVVBSCg==

    bandit10@melinda:~$ base64 --decode data.txt
    The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
```    

####level 11 to Level 12

* username = bandit11
* password = IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR

  ######Things we have to do and the results
  the password is encoded using simple rot13 encryption

```  
    bandit11@melinda:~$ ls
    data.txt
    bandit11@melinda:~$ cat data.txt
    Gur cnffjbeq vf 5Gr8L4qetPEsPk8htqjhRK8XSP6x2RHh
    bandit11@melinda:~$ alias rot13="tr a-zA-Z n-za-mN-ZA-M"

    bandit11@melinda:~$ cat data.txt | rot13
    The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
```  
    

####level 12 to Level 13

* username = bandit12
* password = 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

  ######Things we have to do and the results
  the password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed.
  
```  
bandit12@melinda:~$ ls
data.txt
bandit12@melinda:~$ file data.txt
data.txt: ASCII text
bandit12@melinda:~$ mkdir /tmp/vvv
bandit12@melinda:~$ cd /tmp/vvv
bandit12@melinda:/tmp/vvv$ xxd -r ~/data.txt > data.txt
bandit12@melinda:/tmp/vvv$ file data.txt
data.txt: gzip compressed data, was "data2.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression
bandit12@melinda:/tmp/vvv$ zcat data.txt > dataNew
bandit12@melinda:/tmp/vvv$ ls
data.txt  dataNew
bandit12@melinda:/tmp/vvv$ file dataNew
dataNew: bzip2 compressed data, block size = 900k
bandit12@melinda:/tmp/vvv$ bzip2 -d dataNew
bzip2: Can't guess original name for dataNew -- using dataNew.out
bandit12@melinda:/tmp/vvv$ ls
data.txt  dataNew.out
bandit12@melinda:/tmp/vvv$ file dataNew.out
dataNew.out: gzip compressed data, was "data4.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression
bandit12@melinda:/tmp/vvv$ zcat dataNew.out > evenNewer
bandit12@melinda:/tmp/vvv$ ls
data.txt  dataNew.out  evenNewer
bandit12@melinda:/tmp/vvv$ file evenNewer
evenNewer: POSIX tar archive (GNU)
bandit12@melinda:/tmp/vvv$ tar -xvf evenNewer
data5.bin
bandit12@melinda:/tmp/vvv$ file data5.bin
data5.bin: POSIX tar archive (GNU)
bandit12@melinda:/tmp/vvv$ tar -xvf data5.bin
data6.bin
bandit12@melinda:/tmp/vvv$ file data6.bin
data6.bin: bzip2 compressed data, block size = 900k
bandit12@melinda:/tmp/vvv$ bzip2 -d data6.bin
bzip2: Can't guess original name for data6.bin -- using data6.bin.out
bandit12@melinda:/tmp/vvv$ ls
data.txt  data5.bin  data6.bin.out  dataNew.out  evenNewer
bandit12@melinda:/tmp/vvv$ file data6.bin.out
data6.bin.out: POSIX tar archive (GNU)
bandit12@melinda:/tmp/vvv$ tar -xvf data6.bin.out
data8.bin
bandit12@melinda:/tmp/vvv$ file data8.bin
data8.bin: gzip compressed data, was "data9.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression
bandit12@melinda:/tmp/vvv$ zcat data8.bin > lost
bandit12@melinda:/tmp/vvv$ ls
data.txt  data5.bin  data6.bin.out  data8.bin  dataNew.out  evenNewer  lost
bandit12@melinda:/tmp/vvv$ file lost
lost: ASCII text
bandit12@melinda:/tmp/vvv$ cat lost
```  

  
  
####level 13 to Level 14

* username = bandit13
* password = 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

  ######Things we have to do and the results
  The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14

```  
bandit12@melinda:~$ ls
data.txt
bandit12@melinda:~$ file data.txt
data.txt: ASCII text
bandit12@melinda:~$ mkdir /tmp/vvv
bandit12@melinda:~$ cd /tmp/vvv
bandit12@melinda:/tmp/vvv$ xxd -r ~/data.txt > data.txt
bandit12@melinda:/tmp/vvv$ file data.txt
data.txt: gzip compressed data, was "data2.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression
bandit12@melinda:/tmp/vvv$ zcat data.txt > dataNew
bandit12@melinda:/tmp/vvv$ ls
data.txt  dataNew
bandit12@melinda:/tmp/vvv$ file dataNew
dataNew: bzip2 compressed data, block size = 900k
bandit12@melinda:/tmp/vvv$ bzip2 -d dataNew
bzip2: Can't guess original name for dataNew -- using dataNew.out
bandit12@melinda:/tmp/vvv$ ls
data.txt  dataNew.out
bandit12@melinda:/tmp/vvv$ file dataNew.out
dataNew.out: gzip compressed data, was "data4.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression
bandit12@melinda:/tmp/vvv$ zcat dataNew.out > evenNewer
bandit12@melinda:/tmp/vvv$ ls
data.txt  dataNew.out  evenNewer
bandit12@melinda:/tmp/vvv$ file evenNewer
evenNewer: POSIX tar archive (GNU)
bandit12@melinda:/tmp/vvv$ tar -xvf evenNewer
data5.bin
bandit12@melinda:/tmp/vvv$ file data5.bin
data5.bin: POSIX tar archive (GNU)
bandit12@melinda:/tmp/vvv$ tar -xvf data5.bin
data6.bin
bandit12@melinda:/tmp/vvv$ file data6.bin
data6.bin: bzip2 compressed data, block size = 900k
bandit12@melinda:/tmp/vvv$ bzip2 -d data6.bin
bzip2: Can't guess original name for data6.bin -- using data6.bin.out
bandit12@melinda:/tmp/vvv$ ls
data.txt  data5.bin  data6.bin.out  dataNew.out  evenNewer
bandit12@melinda:/tmp/vvv$ file data6.bin.out
data6.bin.out: POSIX tar archive (GNU)
bandit12@melinda:/tmp/vvv$ tar -xvf data6.bin.out
data8.bin
bandit12@melinda:/tmp/vvv$ file data8.bin
data8.bin: gzip compressed data, was "data9.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression
bandit12@melinda:/tmp/vvv$ zcat data8.bin > lost
bandit12@melinda:/tmp/vvv$ ls
data.txt  data5.bin  data6.bin.out  data8.bin  dataNew.out  evenNewer  lost
bandit12@melinda:/tmp/vvv$ file lost
lost: ASCII text
bandit12@melinda:/tmp/vvv$ cat lost
    4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
```
    
    
####level 14 to Level 15

* username = bandit14
* password = 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e

  ######Things we have to do and the results
  the password for the next level can be retrieved by submitting the password of the current level to port 30000 on localhost
  
```  
    bandit14@melinda:~$ echo 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e | nc -v localhost 30000
    Connection to localhost 30000 port [tcp/*] succeeded!
    Correct!
    BfMYroe26WYalil77FoDi9qh59eK5xNr
```
    
    
####level 15 to Level 16

* username = bandit15
* password = BfMYroe26WYalil77FoDi9qh59eK5xNr

  ######Things we have to do and the results
  The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL encryption
  
```  
    bandit15@melinda:~$ echo BfMYroe26WYalil77FoDi9qh59eK5xNr | openssl s_client -quiet -connect localhost:30001
    depth=0 CN = localhost
    verify error:num=18:self signed certificate
    verify return:1
    depth=0 CN = localhost
    verify return:1
    Correct!
    cluFn7wTiGryunymYOu4RcffSxQluehd
    read:errno=0
```
    
####level 16 to Level 17

* username = bandit16
* password = cluFn7wTiGryunymYOu4RcffSxQluehd

  ######Things we have to do and the results
  
```  
    bandit16@melinda:~$ nmap -sT localhost -p31000-32000
    
    Starting Nmap 5.21 ( http://nmap.org ) at 2015-08-19 09:25 UTC
    Nmap scan report for localhost (127.0.0.1)
    Host is up (0.0013s latency).
    Not shown: 996 closed ports
    PORT      STATE SERVICE
    31046/tcp open  unknown
    31518/tcp open  unknown
    31691/tcp open  unknown
    31790/tcp open  unknown
    31960/tcp open  unknown
    bandit16@melinda:~$ echo test | nc -v localhost 31046
    Connection to localhost 31046 port [tcp/*] succeeded!
    test
    bandit16@melinda:~$ echo test | nc -v localhost 31518
    Connection to localhost 31518 port [tcp/*] succeeded!
    ERROR
    140737354069664:error:1408F10B:SSL routines:SSL3_GET_RECORD:wrong version number:s3_pkt.c:348:
    bandit16@melinda:~$ echo test | nc -v localhost 31691
    Connection to localhost 31691 port [tcp/*] succeeded!
    test
    bandit16@melinda:~$ echo test | nc -v localhost 31790
    Connection to localhost 31790 port [tcp/*] succeeded!
    ERROR
    140737354069664:error:1408F10B:SSL routines:SSL3_GET_RECORD:wrong version number:s3_pkt.c:348:
    bandit16@melinda:~$ echo test | nc -v localhost 31960
    Connection to localhost 31960 port [tcp/*] succeeded!
    test
    bandit16@melinda:~$ echo cluFn7wTiGryunymYOu4RcffSxQluehd | openssl s_client -quiet -connect localhost:31518
    depth=0 CN = localhost
    verify error:num=18:self signed certificate
    verify return:1
    depth=0 CN = localhost
    verify return:1
    cluFn7wTiGryunymYOu4RcffSxQluehd
    
    bandit16@melinda:~$ echo cluFn7wTiGryunymYOu4RcffSxQluehd | openssl s_client -quiet -connect localhost:31790
    depth=0 CN = localhost
    verify error:num=18:self signed certificate
    verify return:1
    depth=0 CN = localhost
    verify return:1
    Correct!
    
    read:errno=0
    bandit16@melinda:~$ mkdir -p /tmp/key/
    bandit16@melinda:~$ cd /tmp/key/
    bandit16@melinda:/tmp/key$ touch sshkey.private
    bandit16@melinda:/tmp/key$ vim sshkey.private
 
    bandit16@melinda:/tmp/key$ ssh -i ./sshkey.private bandit17@localhost
    ...
    Are you sure you want to continue connecting (yes/no)? yes
```


####level 17 to Level 18
* username = bandit17
* password = cluFn7wTiGryunymYOu4RcffSxQluehd


  ######Things we have to do and the results

```  
    bandit17@melinda:~$ ls
    passwords.new  passwords.old
    bandit17@melinda:~$ diff passwords.new passwords.old
    42c42
    < kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
    ---
    > PRjrhDcANrVM6em57fPnFp4Tcq8gvwzK
```    
   
    
####level 18 to Level 19

* username = bandit18
* password = kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd

 ######Things we have to do and the results
``` 
 Byebye !
Connection to bandit.labs.overthewire.org closed.

[root@localhost Desktop]# ssh bandit18@bandit.labs.overthewire.org cat readme
bandit18@bandit.labs.overthewire.org's password: 
IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x
```


####level 19 to Level 20

* username = bandit19
* password = GbKksEFF4yrVs6il55v6gwY5aVje5f0j

```
 ######Things we have to do and the results
 
bandit19@melinda:~$ ls
bandit20-do
bandit19@melinda:~$ ./bandit20-do
Run a command as another user.
  Example: ./bandit20-do id
bandit19@melinda:~$ ./bandit20-do id
uid=11019(bandit19) gid=11019(bandit19) euid=11020(bandit20) groups=11020(bandit20),11019(bandit19)
bandit19@melinda:~$ ./bandit20-do whoami
bandit20
bandit19@melinda:~$ ./bandit20-do cat /etc/bandit_pass/bandit20
GbKksEFF4yrVs6il55v6gwY5aVje5f0j
```

    
    

