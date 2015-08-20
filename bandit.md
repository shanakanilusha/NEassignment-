####Level 0

* username = bandit0
* password = bandit0


####level 0 to Level 1

* username = bandit0
* password = bandit0

  ######Things we have to do and the results

    bandit0@melinda:~$ ls
    readme

    bandit0@melinda:~$ cat readme 
    boJ9jbbUNNfktd78OOpsqOltutMc3MY1


####level 1 to Level 2

* username = bandit1
* password = boJ9jbbUNNfktd78OOpsqOltutMc3MY1

  ######Things we have to do and the results 

    bandit1@melinda:~$ ls
    -

    bandit1@melinda:~$ cat ./\- 
    CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9


####level 2 to Level 3

* username = bandit2
* password = CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

  ######Things we have to do and the results

    bandit2@melinda:~$ ls
    spaces in this filename


    bandit2@melinda:~$ cat ./spaces\ in\ this\ filename 
    UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
    
    
####level 3 to Level 4

* username = bandit3
* password = UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

  ######Things we have to do and the results
    bandit3@melinda:~$ ls
    inhere

    bandit3@melinda:~$ cd inhere/
    bandit3@melinda:~/inhere$ ls

    bandit3@melinda:~/inhere$ ls -al
    total 12
    drwxr-xr-x 2 root    root    4096 Jun  6  2013 .
    drwxr-xr-x 3 root    root    4096 Jun  6  2013 ..
    -rw-r----- 1 bandit4 bandit3   33 Jun  6  2013 .hidden

    bandit3@melinda:~/inhere$ cat .hidden 
    pIwrPrtPN36QITSp3EQaw936yaFoFgAB
    
    
    

####level 4 to Level 5

* username = bandit4
* password = pIwrPrtPN36QITSp3EQaw936yaFoFgAB

  ######Things we have to do and the results
    bandit4@melinda:~$ ls
    inhere

    bandit4@melinda:~$ cd inhere/
    bandit4@melinda:~/inhere$ ls
    -file00  -file01  -file02  -file03  -file04  -file05  -file06  -file07  -file08  -file09

    bandit4@melinda:~/inhere$ for f in ./*; do cat $f; done;
    �S�U� �&� �?�?ɦ�7 ��n�| ����/�$�Q�J
    ��NO2���s�� =\�� 1�OF��
    4��<�o�l�����՚�~{b�W�$�s<��~(����Å�8��b
    dhz��c�
    g7�!�x �Ӈ��Eo[� �B�
    ���& 6] �U �w޽RZ!N�o�h��)�'߳e�l�?-p#��s ���~�$�������<��Dj�N#C � �0�|���T����G�@���koReBOKuIDDepwhWk7jZC0RTdopnAYKh
    ��d C�g�b�.< ��"Q 2B����{����3S�~і�����|�M�^߮�-%ƌ
  

####level 5 to Level 6

* username = bandit5
* password = koReBOKuIDDepwhWk7jZC0RTdopnAYKh

  ######Things we have to do and the results
    bandit5@melinda:~$ ls
    inhere

    bandit5@melinda:~/inhere$ ls
    maybehere00  maybehere02  maybehere04  maybehere06  maybehere08  maybehere10 
    maybehere12  maybehere14  maybehere16  maybehere18
    maybehere01  maybehere03  maybehere05  maybehere07  maybehere09  maybehere11 
    maybehere13  maybehere15  maybehere17  maybehere19

    bandit5@melinda:~/inhere$ find -readable -size 1033c ! -executable
    ./maybehere07/.file2

    bandit5@melinda:~/inhere$ cat ./maybehere07/.file2
    DXjZPULLxYr17uwoI01bNLQbtFemEgo7


####level 6 to Level 7

* username = bandit6
* password = DXjZPULLxYr17uwoI01bNLQbtFemEgo7

  ######Things we have to do and the results
    bandit6@melinda:~$ find / -user bandit7 -group bandit6 -size 33c 2>&1 | grep -v -F Permission
    /var/lib/dpkg/info/bandit7.password

    bandit6@melinda:~$ cat /var/lib/dpkg/info/bandit7.password
    HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
    
    
####level 7 to Level 8

* username = bandit7
* password = HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

  ######Things we have to do and the results
    bandit7@melinda:~$ ls
    data.txt

    bandit7@melinda:~$ grep millionth data.txt
    millionth cvX2JJa4CFALtqS87jk27qwqGhBM9plV
    
####level 8 to Level 9

* username = bandit8
* password = cvX2JJa4CFALtqS87jk27qwqGhBM9plV

  ######Things we have to do and the results

    bandit8@melinda:~$ ls
    data.txt

    bandit8@melinda:~$ sort data.txt | uniq --count | grep "1 "
    1 UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
    
    
####level 9 to Level 10

* username = bandit9
* password = UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

  ######Things we have to do and the results
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
    
    
####level 10 to Level 11

* username = bandit10
* password = truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk

  ######Things we have to do and the results
    bandit10@melinda:~$ ls
    data.txt
    bandit10@melinda:~$ cat data.txt
    VGhlIHBhc3N3b3JkIGlzIElGdWt3S0dzRlc4TU9xM0lSRnFyeEUxaHhUTkViVVBSCg==

    bandit10@melinda:~$ base64 --decode data.txt
    The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
    

####level 11 to Level 12

* username = bandit11
* password = IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR

  ######Things we have to do and the results
    bandit11@melinda:~$ ls
    data.txt
    bandit11@melinda:~$ cat data.txt
    Gur cnffjbeq vf 5Gr8L4qetPEsPk8htqjhRK8XSP6x2RHh
    bandit11@melinda:~$ alias rot13="tr a-zA-Z n-za-mN-ZA-M"

    bandit11@melinda:~$ cat data.txt | rot13
    The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
    

####level 12 to Level 13

* username = bandit12
* password = 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu

  ######Things we have to do and the results
{
 }
    bandit12@melinda:~$ ls
    data.txt
    bandit12@melinda:~$ cat data.txt
    0000000:	1f8b	0808	d095	b051	0203	6461	7461	322e	.......Q..data2.
    0000010:	6269	6e00	013a	02c5	fd42	5a68	3931	4159	bin..:...BZh91AY
    0000020:	2653	5915	d9db	2800	0017	7fff	ff5d	f6ea	&SY...(......]..
    0000030:	e98b	bff6	ff7f	ffbf	fce3	f7fa	a3fb	badb	................
 {

  }    
    bandit12@melinda:/tmp/simple-plan$ cat data8 
    The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
  
  
####level 13 to Level 14

* username = bandit13
* password = 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

  ######Things we have to do and the results
  bandit13@melinda:~$ ls
    sshkey.private
    bandit13@melinda:~$ cat sshkey.private
    -----BEGIN RSA PRIVATE KEY-----
    MIIEpAIBAAKCAQEAxkkOE83W2cOT7IWhFc9aPaaQmQDdgzuXCv+ppZHa++buSkN+
    gg0tcr7Fw8NLGa5+Uzec2rEg0WmeevB13AIoYp0MZyETq46t+jk9puNwZwIt9XgB
    ZufGtZEwWbFWw/vVLNwOXBe4UWStGRWzgPpEeSv5Tb1VjLZIBdGphTIK22Amz6Zb
{
}
    bandit13@melinda:~$ ssh -i ./sshkey.private bandit14@localhost
    Could not create directory '/home/bandit13/.ssh'.
    The authenticity of host 'localhost (127.0.0.1)' can't be established.
    ECDSA key fingerprint is 91:b4:28:0b:9a:4d:0c:b6:39:1f:8f:68:89:4a:ce:92.
    Are you sure you want to continue connecting (yes/no)? yes
    
    bandit14@melinda:~$ cat /etc/bandit_pass/bandit14
    4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
    
    
####level 14 to Level 15

* username = bandit14
* password = 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e

  ######Things we have to do and the results
    bandit14@melinda:~$ echo 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e | nc -v localhost 30000
    Connection to localhost 30000 port [tcp/*] succeeded!
    Correct!
    BfMYroe26WYalil77FoDi9qh59eK5xNr
    
    
####level 15 to Level 16

* username = bandit15
* password = BfMYroe26WYalil77FoDi9qh59eK5xNr

  ######Things we have to do and the results
    bandit15@melinda:~$ echo BfMYroe26WYalil77FoDi9qh59eK5xNr | openssl s_client -quiet -connect localhost:30001
    depth=0 CN = localhost
    verify error:num=18:self signed certificate
    verify return:1
    depth=0 CN = localhost
    verify return:1
    Correct!
    cluFn7wTiGryunymYOu4RcffSxQluehd
    read:errno=0
    
####level 16 to Level 17

* username = bandit16
* password = cluFn7wTiGryunymYOu4RcffSxQluehd

  ######Things we have to do and the results
    bandit16@melinda:~$ nmap -sT localhost -p31000-32000
    
    Starting Nmap 5.21 ( http://nmap.org ) at 2014-01-22 09:25 UTC
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


####level 17 to Level 18


  ######Things we have to do and the results
    bandit17@melinda:~$ ls
    passwords.new  passwords.old
    bandit17@melinda:~$ diff passwords.new passwords.old
    42c42
    < kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
    ---
    > PRjrhDcANrVM6em57fPnFp4Tcq8gvwzK
    
    
####level 18 to Level 19

* username = bandit18
* password = kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd

 
    
    

