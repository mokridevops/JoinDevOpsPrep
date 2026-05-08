
tar command: tar - tap or disc archive
------------
.zip -> compressin format

.tar.gz -> linux format

tar -

<img width="1029" height="658" alt="image" src="https://github.com/user-attachments/assets/3d39bfa5-4897-4aad-9ec7-ff0d5d4780fd" />


<img width="888" height="636" alt="image" src="https://github.com/user-attachments/assets/f5b0c5fe-c10f-47e2-8638-9e9229f142cb" />


when an employee leaves the organization:

1. lock the user, remove him from all the groups
2. if he already logged in, forc logout him
3. take back up of his ifle, including his home directoy
4. remove his home folder
5. check if he has entry in sudoers file or sudoers.d (directory)

usermod --help | grep lock

usermod -L ramesh

gpasswd -d ramesh testers

usermod -g ramesh ramesh

mkdir /backup

tar -czvf ramesh_homedir.tar.gz /home/ramesh



<img width="1062" height="477" alt="image" src="https://github.com/user-attachments/assets/887662bc-5c5e-48d9-a337-eac84ae631eb" />

package management:
-------------------

For Redhat:

dnf install <package-name>
dnf remove <package-name>

dnf update <package-name> - if there are any new version in that package

dnf search <package-name>
dnf info <package-name>

dnf list installed  | grep nginx
dnf list available -> not insatlled in the system, but available in cloud

dnf list available | wc -l

dnf remove -y

dnf repolist -> lists all repositories
apt-get -> debian family



Service managment:
------------------

sshd -> service, continously running doing some work

systemctl start <service-name>

nginx -> popular web/http server

dnf install nginx -y
systemctl start nginx
systemctl status nginx

systemctl stop nginx
system status nginx
systectl restart nginx
systemctl enable nginx - if you start the server, it will automatically start
systemctl disable nginx -> disabling auto start



Process management:
-------------------

ticket creation -> cisual in ap
ticket done -> update

ticket_id 

every process is tracked thorugh id - process-id

lead -> senior -> junior -> fresher

a process can start another process.

pid -> process instance id -> child
ppid -> parent process instance id


ps - list the processes of current logged in user

ps aux - to see all process with user names, and cpu, ram, etc in the system

ps -ef -> PID, PPID (this is like task manager) -> all processes information along with parents

ps -u ecu2-user -> gives all the processes that are started by ec2-user

top - all processes - in live

htop 

top -u ec2-user


there are two types of process:
1.background process
2.foreground process


sleep 5  -> foreground process


<img width="1031" height="207" alt="image" src="https://github.com/user-attachments/assets/098c3eb0-7756-4da0-b8fa-88fe5a9d1912" />

it sleeps for 60s in background and then comes back

kill 28683 

kill -9 28740  (force kill)

<img width="507" height="81" alt="image" src="https://github.com/user-attachments/assets/e24d9f68-2c02-41be-afe1-fd6da305b997" />



Network Managment:
------------------

ntetstat -lntp -> ports opened in our server

what ever port numbers that are opened in our system


sudo systemctl start nginx


systemctl status 
netstat -lntp
ps -ef | grep <service-name>

---------------

Projects:

3 tier architecture
-------------------
1 person he has food items
   taking order, cooking, taking payments, queue maintenance, 
   max : 5 - 10 members


hotel model
----------
token system -> taking payments
cooks -> keep the orders in queue, cook and serve them
max: 20 members


restaurant model
----------------

captain -> welcome us
he checks which table is free
table -> waiter
chef -> only cooking
max: 100 - 200

Web tier / frontend tier
-----------------------
load balancer
frontend -> html, javascript, css

backend tier/ app tier
----------------------
backend -> java, python, .net, nodejs, go, etc

database tier
-------------
database -> user data -> mysql, oracle, postgres, MSSQL, etc

{ 
"user" : "sivakumar",
"email": "info@joindevops.com"
}

   

















