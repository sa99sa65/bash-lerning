## ki ki file and folder ase sob dekar jonno ls command dei 

sajjad@sajjad:~$ ls

 am.sh       Documents   Music       shell_resources   today
 cmp         Downloads   Pictures    snap             'Untitled Document 1'
 curentdir   Public      StudioProjects    Videos
 Desktop     first.sh    README.md   Templates

##Desktop move korbar jonno ei command ta liki 

sajjad@sajjad:~$ cd desktop

bash: cd: desktop: No such file or directory


sajjad@sajjad:~$ cd Desktop


sajjad@sajjad:~/Desktop$ ls

 apple   bvd   efg   f1_299.txt   fr   hello.sh  'New Folder'   pear   saj
 
 ##ami directly desktop taki file open korar try korsi its give wrong 
 
sajjad@sajjad:~/Desktop$ hello.sh
hello.sh: command not found


sajjad@sajjad:~/Desktop$ cd hello.sh
bash: cd: hello.sh: Not a directory

## amar kun bash ase bah ami file use korbo seta lika jonno ei command use korle amake dekave 

sajjad@sajjad:~/Desktop$ which bash
/usr/bin/bash

##amra jani j root firbar jonno amra cd .. use kori

sajjad@sajjad:~/Desktop$ cd ..

sajjad@sajjad:~$ which bash
/usr/bin/bash

sajjad@sajjad:~$ cd Desktop

## ami script run korbar jonno akta file kultesi tobe must deko ami file sese kisu extension disi (.sh)

sajjad@sajjad:~/Desktop$ touch sajjadScript.sh

sajjad@sajjad:~/Desktop$ cat  sajjadScript.sh
sajjad@sajjad:~/Desktop$ hi
Command 'hi' not found, but can be installed with:
sudo snap install hi

##ls -all diya ami amar script er mode ta cheak kore nisi 

sajjad@sajjad:~/Desktop$ ls -al
total 24
drwxr-xr-x  4 sajjad sajjad 4096 ডিসেম্বর   2 12:42  .
drwxr-x--- 27 sajjad sajjad 4096 নভেম্বর    5 00:08  ..
drwxrwxr-x  2 sajjad sajjad 4096 ডিসেম্বর   2 12:42  fr
-rwxrwxr-x  1 sajjad sajjad 1225 নভেম্বর    5 06:28  hello.sh
drwxrwxr-x  2 sajjad sajjad 4096 সেপ্টেম্বর 14 09:40 'New Folder'
-rw-rw-r--  1 sajjad sajjad   39 ডিসেম্বর   2 12:41  sajjadScript.sh

## now I changed the mode of this file for i can write something 
##-- clear define see the line [ 65 and 77 ]
sajjad@sajjad:~/Desktop$ chmod +x sajjadScript.sh
sajjad@sajjad:~/Desktop$ ls -al
total 24
drwxr-xr-x  4 sajjad sajjad 4096 ডিসেম্বর   2 12:42  .
drwxr-x--- 27 sajjad sajjad 4096 নভেম্বর    5 00:08  ..
drwxrwxr-x  2 sajjad sajjad 4096 ডিসেম্বর   2 12:42  fr
-rwxrwxr-x  1 sajjad sajjad 1225 নভেম্বর    5 06:28  hello.sh
drwxrwxr-x  2 sajjad sajjad 4096 সেপ্টেম্বর 14 09:40 'New Folder'
-rwxrwxr-x  1 sajjad sajjad   39 ডিসেম্বর   2 12:41  sajjadScript.sh

## oh no , I am sorry to mentions that whenever I want create a file I must put this command in the intial file 
## [ #! /usr/bin/bash ] i find it from which bash command 


## now i wanna print the file so simple i run the command [ ./filename.sh ] 

sajjad@sajjad:~/Desktop$ ./sajjadScript.sh
hello sajjad 
sajjad@sajjad:~/Desktop$ cat /home/user/.bash_history
cat: /home/user/.bash_history: No such file or directory
sajjad@sajjad:~/Desktop$ ls
 fr   hello.sh  'New Folder'   sajjadScript.sh
sajjad@sajjad:~/Desktop$ cat ~/.bash_history > history_backup
sajjad@sajjad:~/Desktop$ 
