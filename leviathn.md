####level 0 to Level 1

* username = Leviathan0
* password = rioGegei8m

######Description and the code
Firt of all we have to make a SSH connection to "leviathan.labs.overthewire.org".After that we have log into Leviathan0’s shell, we should look around. Upon inspection of our home directory, we see a backup directory named to be hidden. Taking a closer look of what is contained in the backup easily reveals the password to get into level 1 and begin leviathan.
```
leviathan0@melinda:~$ ls -la
total 24
drwxr-xr-x   3 root       root       4096 Nov 14  2014 .
drwxr-xr-x 167 root       root       4096 Jul  9 16:27 ..
drwxr-x---   2 leviathan1 leviathan0 4096 Jul 17 16:44 .backup
-rw-r--r--   1 root       root        220 Apr  9  2014 .bash_logout
-rw-r--r--   1 root       root       3637 Apr  9  2014 .bashrc
-rw-r--r--   1 root       root        675 Apr  9  2014 .profile

leviathan0@melinda:~$ cd .backup/
leviathan0@melinda:~/.backup$ cat bookmarks.html | grep password
<DT><A HREF="http://leviathan.labs.overthewire.org/passwordus.html | This will be fixed later, the password for leviathan1 is rioGegei8m" ADD_DATE="1155384634" LAST_CHARSET="ISO-8859-1" ID="rdf:#$2wIU71">password to leviathan1</A>
leviathan0@melinda:~/.backup$

leviathan0@melinda:~/.backup$ cd
leviathan0@melinda:~$ ls
leviathan0@melinda:~$ cd /etc/leviathan_pass/
leviathan0@melinda:/etc/leviathan_pass$ ls
leviathan0  leviathan2  leviathan4  leviathan6
leviathan1  leviathan3  leviathan5  leviathan7
leviathan0@melinda:/etc/leviathan_pass$
```

####level 1 to Level 2

* username = Leviathan1
* password = ougahZi8Ta

######Description and the code

Leviathan 1 presents in the home directory as binary. If we run it we see that is a utility that ask and checks for a password.
```
leviathan1@melinda:~$ ./check
password: love
Wrong password, Good Bye ...
leviathan1@melinda:~$ ltrace ./check
__libc_start_main(0x804852d, 1, 0xffffd7a4, 0x80485f0 <unfinished ...>
printf("password: ")                              = 10
getchar(0x8048680, 47, 0x804a000, 0x8048642password: love
)      = 108
getchar(0x8048680, 47, 0x804a000, 0x8048642)      = 111
getchar(0x8048680, 47, 0x804a000, 0x8048642)      = 118
strcmp("lov", "sex")                              = -1
puts("Wrong password, Good Bye ..."Wrong password, Good Bye ...
)              = 29
+++ exited (status 0) +++
leviathan1@melinda:~$

leviathan1@melinda:~$ ./check
password: sex
$ whoami
leviathan2
$ cat /etc/leviathan_pass/leviathan2
ougahZi8Ta
$
```

####level 2 to Level 3

* username = Leviathan2
* password = Ahdiemoo1j

######Description and the code
Leviathan2 has the password to access the leviathan3, it contains in a small binary that belongs to the user leviathan3 and group leviathan2.

```
leviathan2@melinda:~$ ls -la
total 28
drwxr-xr-x   2 root       root       4096 Nov 14  2014 .
drwxr-xr-x 167 root       root       4096 Jul  9 16:27 ..
-rw-r--r--   1 root       root        220 Apr  9  2014 .bash_logout
-rw-r--r--   1 root       root       3637 Apr  9  2014 .bashrc
-rw-r--r--   1 root       root        675 Apr  9  2014 .profile
-r-sr-x---   1 leviathan3 leviathan2 7498 Nov 14  2014 printfile

leviathan2@melinda:~$ ./printfile
*** File Printer ***
Usage: ./printfile filename
leviathan2@melinda:~$

leviathan2@melinda:~$ mkdir /tmp/solveme && touch /tmp/solveme/file\ tmp.txt
leviathan2@melinda:~$ cd /tmp/solveme
leviathan2@melinda:/tmp/solveme$ ls -ls
total 0
0 lrwxrwxrwx 1 leviathan2 leviathan2 30 Oct  3 17:22 file -> /etc/leviathan_pass/leviathan3
0 -rw-rw-r-- 1 leviathan2 leviathan2  0 Oct  3 17:18 file tmp.txt
leviathan2@melinda:/tmp/solveme$
leviathan2@melinda:/tmp/solveme$ ltrace ~/printfile "fie tmp.txt"
__libc_start_main(0x804852d, 2, 0xffffd744, 0x8048600 <unfinished ...>
access("fie tmp.txt", 4)                          = -1
puts("You cant have that file..."You cant have that file...
)                = 27
+++ exited (status 1) +++
leviathan2@melinda:/tmp/solveme$
```

####level 3 to Level 4

* username = Leviathan3
* password = vuH0coox6m

######Description, codes and the outputs
We only need a few commands to get access to Leviathan4. When we finally do get its shell, we can "cat" its password in /etc/leviathan_pass/leviathan4.

```
leviathan3@melinda:~$ ls
level3
leviathan3@melinda:~$ ./level3
Enter the password> passward
bzzzzzzzzap. WRONG
leviathan3@melinda:~$ string ./level3
-bash: string: command not found
leviathan3@melinda:~$ strings ./level3
/lib/ld-linux.so.2
libc.so.6
_IO_stdin_used
puts
__stack_chk_fail
stdin
printf
fgets
system
strcmp
__libc_start_main
__gmon_start__
GLIBC_2.4
GLIBC_2.0
PTRh@
snlp
rintf
D$L1
D$#bombf
D$'ad
D$8...s
D$<3cr3f
D$@t
D$*h0nof
D$.33
D$1kakaf
D$5ka
D$B*32.
D$F2*[xf
D$J]
T$Le3
[^_]
[You've got shell]!
/bin/sh
bzzzzzzzzap. WRONG
Enter the password>
;*2$"
secret
GCC: (Ubuntu 4.8.2-19ubuntu1) 4.8.2
/usr/lib/gcc/x86_64-linux-gnu/4.8/include
/usr/include/bits
/usr/include
level3.c
stddef.h
types.h
libio.h
stdio.h
__off_t
_IO_read_ptr
_chain
do_stuff
size_t
_shortbuf
_IO_buf_base
long long unsigned int
long long int
other
_fileno
_IO_read_end
_flags
_IO_buf_end
_cur_column
__quad_t
_old_offset
level3.c
_IO_marker
stdin
_IO_write_ptr
_sbuf
short unsigned int
_IO_save_base
kaka
_lock
_flags2
_mode
sizetype
_IO_write_end
kaka2
_IO_lock_t
_IO_FILE
GNU C 4.8.2 -m32 -mtune=generic -march=i686 -g -fstack-protector
_pos
_markers
unsigned char
short int
asdf
_vtable_offset
_next
__off64_t
_IO_read_base
_IO_save_end
/root/OverTheWire-games/games/leviathan/leviathan3
__pad1
__pad2
__pad3
__pad4
__pad5
_unused2
morenothing
_IO_backup_base
main
_IO_write_base
.symtab
.strtab
.shstrtab
.interp
.note.ABI-tag
.note.gnu.build-id
.gnu.hash
.dynsym
.dynstr
.gnu.version
.gnu.version_r
.rel.dyn
.rel.plt
.init
.text
.fini
.rodata
.eh_frame_hdr
.eh_frame
.init_array
.fini_array
.jcr
.dynamic
.got
.got.plt
.data
.bss
.comment
.debug_aranges
.debug_info
.debug_abbrev
.debug_line
.debug_str
crtstuff.c
__JCR_LIST__
deregister_tm_clones
register_tm_clones
__do_global_dtors_aux
completed.6590
__do_global_dtors_aux_fini_array_entry
frame_dummy
__frame_dummy_init_array_entry
level3.c
__FRAME_END__
__JCR_END__
__init_array_end
_DYNAMIC
__init_array_start
_GLOBAL_OFFSET_TABLE_
__libc_csu_fini
strcmp@@GLIBC_2.0
_ITM_deregisterTMCloneTable
__x86.get_pc_thunk.bx
data_start
printf@@GLIBC_2.0
fgets@@GLIBC_2.0
_edata
_fini
__stack_chk_fail@@GLIBC_2.4
__data_start
puts@@GLIBC_2.0
system@@GLIBC_2.0
__gmon_start__
__dso_handle
_IO_stdin_used
__libc_start_main@@GLIBC_2.0
__libc_csu_init
stdin@@GLIBC_2.0
_end
_start
_fp_hw
nothing
__bss_start
main
_Jv_RegisterClasses
__TMC_END__
_ITM_registerTMCloneTable
do_stuff
_init
leviathan3@melinda:~$

leviathan3@melinda:~$ ./level3
Enter the password> snlprintf
[You've got shell]!
$ whoami
leviathan4
$ cat /etc/leviathan_pass/leviathan4
vuH0coox6m
$
```

####level 4 to level 5

* username = Leviathan4
* password = passwaor is in binary format so we have to convert it,"01010100 01101001 01110100 01101000 00110100 01100011 01101111 01101011 01100101 01101001 00001010"
              (Tith4cokei)

######Description, codes and the outputs
There is a trash directory. Navigate to it to find a binary aptly named “bin”. After running it, we see sets of binary code as output.

```
leviathan4@melinda:~$ ls -la
total 24
drwxr-xr-x   3 root root       4096 Nov 14  2014 .
drwxr-xr-x 167 root root       4096 Jul  9 16:27 ..
-rw-r--r--   1 root root        220 Apr  9  2014 .bash_logout
-rw-r--r--   1 root root       3637 Apr  9  2014 .bashrc
-rw-r--r--   1 root root        675 Apr  9  2014 .profile
dr-xr-x---   2 root leviathan4 4096 Nov 14  2014 .trash
leviathan4@melinda:~$

leviathan4@melinda:~$ cd .trash/
leviathan4@melinda:~/.trash$ ls -la
total 16
dr-xr-x--- 2 root       leviathan4 4096 Nov 14  2014 .
drwxr-xr-x 3 root       root       4096 Nov 14  2014 ..
-r-sr-x--- 1 leviathan5 leviathan4 7425 Nov 14  2014 bin
leviathan4@melinda:~/.trash$

leviathan4@melinda:~/.trash$ ./bin
01010100 01101001 01110100 01101000 00110100 01100011 01101111 01101011 01100101 01101001 00001010
leviathan4@melinda:~/.trash$
```

####level 5 to Level 6

* username = Leviathan5
* password = UgaoFee4li

######Description, codes and the outputs
 we have to exploit the binary by using using symbolic linking to a file we have permission of. When we run the binary in Leviathan5’s home directory, it appears to be attempting to read from a file in /tmp. 

```
leviathan5@melinda:~$ ls -la
total 28
drwxr-xr-x   2 root       root       4096 Nov 14  2014 .
drwxr-xr-x 167 root       root       4096 Jul  9 16:27 ..
-rw-r--r--   1 root       root        220 Apr  9  2014 .bash_logout
-rw-r--r--   1 root       root       3637 Apr  9  2014 .bashrc
-rw-r--r--   1 root       root        675 Apr  9  2014 .profile
-r-sr-x---   1 leviathan6 leviathan5 7634 Nov 14  2014 leviathan5
leviathan5@melinda:~$

leviathan5@melinda:~$ ./leviathan5
Cannot find /tmp/file.log
leviathan5@melinda:~$ ln -s /etc/leviathan_pass/leviathan6 /tmp/file.log
leviathan5@melinda:~$ ./leviathan5
UgaoFee4li
leviathan5@melinda:~$
```
