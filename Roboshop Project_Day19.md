Linux Memory commands:

<img width="1532" height="735" alt="image" src="https://github.com/user-attachments/assets/9ef77f5e-3750-4b4b-9432-60ca43cb376d" />


<img width="918" height="426" alt="image" src="https://github.com/user-attachments/assets/e0ee9505-c1ab-45ea-92b9-1fd30f9cc405" />


top
htop -y


<img width="1096" height="842" alt="image" src="https://github.com/user-attachments/assets/ae0a0b25-1e20-4ebd-b7c4-327d76709386" />
<img width="1542" height="867" alt="image" src="https://github.com/user-attachments/assets/cb8c9ff2-bf20-422b-9292-e5440d784ef7" />


ps -aux


<img width="1515" height="896" alt="image" src="https://github.com/user-attachments/assets/f7b31341-50a7-4478-b882-80b19ff3cf9a" />

ps -aux --sort=%mem 10

gives top 10 memory usage

<img width="1137" height="865" alt="image" src="https://github.com/user-attachments/assets/beb85e0e-0c7a-49db-88e9-2d7c4e50af61" />

top 10 cpu consuming process

<img width="1503" height="885" alt="image" src="https://github.com/user-attachments/assets/c1fb3cd5-5253-4957-8b8f-9ecead20dee2" />


<img width="1472" height="492" alt="image" src="https://github.com/user-attachments/assets/7f0ba794-1041-4c91-9949-e69bc38f04e6" />

Interview questions:

top 10 memory hungry or cpu hungry process

disk usage:
df -hT  -> disk file system information



<img width="988" height="877" alt="image" src="https://github.com/user-attachments/assets/78b369d1-10a3-4fad-a7b3-d46420a4977a" />

<img width="897" height="865" alt="image" src="https://github.com/user-attachments/assets/958abc52-c9e9-4794-9f96-50cfb70ff310" />

<img width="1232" height="487" alt="image" src="https://github.com/user-attachments/assets/6c5c407b-5476-443a-a911-528f66884c8e" />



-------------------


inode symlink and hardlink
--------------------------
Interview questions:


<img width="732" height="336" alt="image" src="https://github.com/user-attachments/assets/50c6ea69-60ff-4ae4-8a82-40eb260e9336" />


symlink - is shortcut in linux

so for files we can create symlink

ln -s 
ln - is link
s - is symlink

ln -s /root/photo.jpg

mkdir /images
ln -s /root/photo.jp images/profile.jpg

ls -l
profile.jpg

<img width="872" height="863" alt="image" src="https://github.com/user-attachments/assets/2e5e7515-4eb0-4e12-bae3-b73fef2bc2bf" />


<img width="915" height="457" alt="image" src="https://github.com/user-attachments/assets/cd63fe86-387b-45cb-aa89-362bcf9feb1b" />


Disk Management:





/image # 












