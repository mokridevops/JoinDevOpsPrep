


<img width="370" height="268" alt="image" src="https://github.com/user-attachments/assets/c53d460b-dcd7-4ba4-b0e6-182a40dbe80b" />

Command <options> <inputs>
usage
uname -> system information
-a -> all system information

/c/devops/daws-90s/repos -> absolute path
repos/ -> relative path

CRUD -> Create Read Update Delete

ls -> list subdirectories

as soon as you login to linux - you will end up in /home/username

/ -> root directory

everything starts from home - in linux

/home -> home directories of linux users
/etc -> configurations
/tmp -> temp files
/bin -> commands or binaries



<img width="874" height="656" alt="image" src="https://github.com/user-attachments/assets/f35a49a0-0f63-4cb7-a0aa-a10b75590568" />

ls -l -> long listing detailed format
ls -lr -> reverse alphabetical format
ls -ltr -> latest files will come at the bottom

<img width="652" height="669" alt="image" src="https://github.com/user-attachments/assets/dd56def3-daf0-458f-a5fc-9b5e0801f9fc" />

hidden files or directories in linux starts with .
ls -la -> all files including hidden

touch <file-name> -> creates empty file

cat devops.txt -> read the file

<img width="537" height="294" alt="image" src="https://github.com/user-attachments/assets/07858aaa-6d1f-4a1d-aca1-572458e43eba" />

<img width="908" height="493" alt="image" src="https://github.com/user-attachments/assets/5b8b630f-00ce-4746-8001-dd48db2d26b2" />

> -> redirection
>
 cat > devops.txt -> read the file

<img width="949" height="568" alt="image" src="https://github.com/user-attachments/assets/aaee9a9a-4591-4b69-8c4b-9e2c2bbb7aaa" />

tac - reverse display

<img width="623" height="518" alt="image" src="https://github.com/user-attachments/assets/3553b81e-985d-4a46-b49a-f9c25afaeb66" />


<img width="1140" height="900" alt="image" src="https://github.com/user-attachments/assets/0a820351-6353-4bdc-924c-116f35f08a43" />


cat > devops.txt -> enter the text ->  enter and ctrl + d

>> -> append
>>
>> cat file-1 file-2 > file-3 => mearge file-1 and file-2 into file-3


<img width="860" height="295" alt="image" src="https://github.com/user-attachments/assets/dc3f42ab-fc25-4ff3-bae4-9564ffd486f4" />

d -> firectory
 - -> file

mkdir -p devops -> if directolry does not exits it wil create, if exits it will be slient no error

rmdir devops -> removes if the directoyr is emtpy

<img width="864" height="604" alt="image" src="https://github.com/user-attachments/assets/d31929fc-ec9a-42e4-97ae-0e4780db652a" />

file-sleet -> ctrl+c -> destination -> ctrl+v

copy:
------
cp <source> <destination>

<img width="836" height="832" alt="image" src="https://github.com/user-attachments/assets/2de729ed-1e6d-4e8b-a025-addd40620908" />

rm -r devops -> recursetly delete filels and directories

<img width="779" height="539" alt="image" src="https://github.com/user-attachments/assets/60f12e6c-72d5-4bc4-acb6-3c80f6cf0ce5" />

thsi is a dangerious operation - it deletes entire folder

<img width="804" height="185" alt="image" src="https://github.com/user-attachments/assets/c3d1df4d-af9e-4d4c-87ab-4bbcc61ddd8c" />

<img width="797" height="621" alt="image" src="https://github.com/user-attachments/assets/8d29a947-b198-4d32-8fa3-580958b983b3" />


How to download the files:
--------------------------
wget <url> -> download the file
curl <url> -> directly shows on the screen (does not download) -> we will use it in scripting and hitting API's
curl -o notes.txt <url> - it is going to put all the contnet of the url in notes.txt - so it is downloading and putting in notes.txt


<img width="1628" height="504" alt="image" src="https://github.com/user-attachments/assets/866bcd32-87a6-41a1-b977-1cf0baf6a36c" />





grep command
-------------
find the text inside files

grep <word-to-find> file-name

<img width="1628" height="504" alt="image" src="https://github.com/user-attachments/assets/d32a0a76-ef21-41d9-9440-80db30f26e16" />

linux , Linux are both different - it is case sensitive



<img width="1118" height="885" alt="image" src="https://github.com/user-attachments/assets/1d754856-2160-4668-a170-73286332e2ea" />

<img width="818" height="130" alt="image" src="https://github.com/user-attachments/assets/dc9cfc54-86c5-4d11-ab1c-9d78c0b9ade3" />

-i -> case insensitive
-n -> line number display
-c -> count number of lines
-v -> opposite, 

grep -v linux file -> not matching linux

piping:
-------

| -> pipe

curl -s 


<img width="1652" height="901" alt="image" src="https://github.com/user-attachments/assets/c803e52b-2073-4729-bf16-233ee57271c7" />



<img width="1658" height="321" alt="image" src="https://github.com/user-attachments/assets/c6a95e8d-30bf-4e33-8340-be9b3a2105cf" />



<img width="1184" height="901" alt="image" src="https://github.com/user-attachments/assets/a57d922a-1d33-444b-9ffb-6aed02d689cb" />

* Interview question

  print lines 10 - 14

  






























