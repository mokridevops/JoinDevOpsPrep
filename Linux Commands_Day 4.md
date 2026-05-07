
VIM Editor:
------------

<img width="593" height="294" alt="image" src="https://github.com/user-attachments/assets/53d210ed-956d-4b56-977c-9a9eec9b931e" />


<img width="1635" height="219" alt="image" src="https://github.com/user-attachments/assets/3b22ac1e-61fc-4899-8000-74e06a0f3b81" />

:set nu -> line numbers

<img width="1117" height="913" alt="image" src="https://github.com/user-attachments/assets/bf9663ce-278a-4fc3-9795-96cf7ebf4020" />

:set nonu -> numbers wil be gone


<img width="1329" height="281" alt="image" src="https://github.com/user-attachments/assets/9e29a10f-24e6-48c5-8c51-9eaa6b9213da" />

:<line-numer> -> cursor will move to that line



<img width="989" height="897" alt="image" src="https://github.com/user-attachments/assets/8a5075db-2409-457f-8753-11189d9e33b4" />

<img width="1061" height="884" alt="image" src="https://github.com/user-attachments/assets/74f1e735-b408-4bb0-ad9b-0a20c75c542d" />

:/<word-to-search> -> this goes forward search

for next word search - you need to press n

reverse search

:?<word-to-search> -> backword search - press n for next search in backward


:2d -> delete line number 2

:2,5d -> deletes lines from 2 - 5

:%d -> deletes all the content in the file, % refers to everything

:noh -> dont highlight the word

<img width="1748" height="643" alt="image" src="https://github.com/user-attachments/assets/e814f78a-5120-41ec-8da5-a8a819bb6371" />

replace any word:

:4s/<word-to-find>/<word-to-replace> - in line-number 4 - replace the first occurance


:/4s/sbin/SBIN/g -> g means all ocurrances in that specific line

:%s/<world-to-find>/<world to replace> -> all line-numbers - replace first occurance

:%s/<world-to-find>/<world to replace>/g -> all line-numbers - replace all occurances



undo the changes: 
u -> undo the changes
ctrl+r -> redo the changes

shift+g -> bottom of the file
shift+gg -> top of the file

<img width="1702" height="793" alt="image" src="https://github.com/user-attachments/assets/be63e4b4-f100-401c-97ad-9b96a520b7a9" />

yy -> copy the line
p -> paste the copied line, under the present cursor line
shift+p -> paste the copied line, above the present cursor line

10p -> paste 10 times


<img width="1713" height="692" alt="image" src="https://github.com/user-attachments/assets/2d7c0cdc-db4a-428c-a2b1-acd4f3320795" />


Linux Administration:
---------------------
1. User Management

IAM - Identity and Access Management

User, Group, Role, Permissions

A group has multiple users
A user have specific role
A role will have permissions

Ramesh - joined devops team, has trainee role , trainee role has particular permissions

roles/sub-groups:
-------
devops-trainee  -> only read access  -> ramesh will be added to this group
devops-juniors  -> he can do specific writes, he cannot udpate, and cannot delete -> ramesh will be moved to this group
devops-seniors  -> write and update
devops-leads    -> write update and delete



Create user -> linux user must have 1 primary group, and 0 - many secondary groups
useradd <username> -> creates user and group with same name
useradd ramesh

id <username>
id ramesh

/etc/password -> user information
/etc/group -> group information

groupadd <group-name>

groupadd devops

cat /etc/group

now add ramesh to that group


User modification
usermod -g <group-name> <user-name> -> -g means primary group

usermod -g devops ramesh
id ramesh

groupadd developers
groupadd testers

usermod -G testers ramesh
id ramesh
usermod -aG developers ramesh  -> a is append - so ramesh is added to developers group apart from testers group, not replacing from testers to developers

<img width="1739" height="760" alt="image" src="https://github.com/user-attachments/assets/8a892f0c-fe87-4904-936e-c46aeb765edd" />

how can you give access to ramesh

passwd ramesh -> to setup password for Ramesh

Linux by default allows key based authentication, if we want password based authentication - we need to edit configuration

ssh config -> /etc/ssh/sshd_config
d means deamon - which will run continously - it cannot be stopped (rakshashi no death)

PasswordAuthentication no
sshd -t -> check for syntax of /etc/ssh/sshd

systemctl restart sshd -> it will restart sshd service

<img width="1022" height="422" alt="image" src="https://github.com/user-attachments/assets/4074e792-e858-4a8e-af70-e47d8feb85c7" />


hwo to give sudo access:
---------------------------
1. add user to wheel group
   usermod -aG wheel ramesh

   id ramesh

   ramesh should logout and login to effect

   sudo useradd suresh - to perform administrative roles

   
   <img width="1274" height="795" alt="image" src="https://github.com/user-attachments/assets/bd310c56-2b98-49a9-9348-4e25c1b015de" />
   

<img width="817" height="409" alt="image" src="https://github.com/user-attachments/assets/08365421-9ef1-43f9-95b2-f6e2c428ba61" />

<img width="966" height="409" alt="image" src="https://github.com/user-attachments/assets/74b77172-e03d-4b9d-991c-5c37f8d14d70" />

<img width="692" height="306" alt="image" src="https://github.com/user-attachments/assets/b1f10b16-d7d3-4c3e-9e80-cc015f4d04c5" />

<img width="1119" height="443" alt="image" src="https://github.com/user-attachments/assets/26225432-7681-4c65-a1fd-590c8ac58a4f" />

<img width="1151" height="219" alt="image" src="https://github.com/user-attachments/assets/3733575c-9204-4d83-886f-856db3fd5a5d" />

Ownership:
--------

chown -> onwer also can't execute this command, only root user can execute

Chown user:group <filename>
chown -R user:group <folder> -> everything inside this folder will get ownership set here

Key-based authentication:
-------------------------
1. ramesh should generate keys
2. he should send his public key to admin team

**<img width="1426" height="710" alt="image" src="https://github.com/user-attachments/assets/dd4efda1-0e4d-44ae-bb7a-be1b671d56d3" />

<img width="973" height="418" alt="image" src="https://github.com/user-attachments/assets/17667e84-0650-4353-a9b1-b22608df85da" />

**






















