
Shell Scripting:

Log_file2.sh

#!/bin/bash

USERID=$(id -u)
# this is to get the id of the root user as an input to our script
LOGS_DIR=/var/log/shell-script
LOGS_FILE="$LOGS_DIR/$0.log" # /var/log/shell-script/log_file2.sh.log

if [ $USERID -ne 0 ]; then
echo "run with root access"
exit 1
fi

VALIDATE()
{
    if [ $2 -ne 0 ]; then
    echo "$2"
    echo "installing $1 is a .... failure"
    exit 1
    else
    echo "installing $1 is a .... success"
    fi
}


echo "I am continuing"
dnf list installed mysql &>> $LOGS_FILE

if [ $? -eq 0 ]; then
    echo "mysql is already installed...Skipping"
else
    echo "installing mysql"
    dnf install mysql -y &>> $LOGS_FILE
    VALIDATE mysql $?
    
fi


dnf list installed nginx &>> $LOGS_FILE

if [ $? -eq 0 ]; then
    echo "nginx is already installed...Skipping"
else
    echo "installing nginx"
    dnf install nginx -y &>> $LOGS_FILE
    VALIDATE nginx $?
fi


<img width="497" height="345" alt="image" src="https://github.com/user-attachments/assets/baf19d97-e43d-4cf4-aee3-560bf9c891e7" />


<img width="406" height="337" alt="image" src="https://github.com/user-attachments/assets/f07f231b-5591-4384-bdb3-c1beec26422c" />

on executing this:

<img width="589" height="92" alt="image" src="https://github.com/user-attachments/assets/7c19ec21-a1c4-4559-8ea9-a274aa666276" />

<img width="611" height="125" alt="image" src="https://github.com/user-attachments/assets/26126fd1-84ba-4c90-8523-ef9da8b16319" />


<img width="557" height="481" alt="image" src="https://github.com/user-attachments/assets/c538ab24-71fd-4678-b457-536772cb8c80" />

all the output is captured in this log file, based on the code that we have given to append the output of the script to this log file:

<img width="434" height="77" alt="image" src="https://github.com/user-attachments/assets/559f7526-0282-498b-abfb-081b92e9566c" />

--------------------------


**tee command:**

Log will be simultaneously printed on terminal and also on the log file



<img width="482" height="363" alt="image" src="https://github.com/user-attachments/assets/5a667ed3-c6b0-487c-a9ff-90024acb003e" />

<img width="464" height="341" alt="image" src="https://github.com/user-attachments/assets/1ac77f89-25bb-4475-a262-ca0ce1cb27fe" />

output:

<img width="594" height="109" alt="image" src="https://github.com/user-attachments/assets/2afc8b0f-7888-494d-960d-d5aa821f27f5" />


<img width="586" height="474" alt="image" src="https://github.com/user-attachments/assets/ec53b16f-0f3e-40b4-9eea-1985141d91c7" />




Loops:
--------------

for number in {1..200}
do 
  statements
done


date format:
-------------

> date +%Y-%m-%d %H:%M%S
>
> you can add this as timestamp:

<img width="614" height="479" alt="image" src="https://github.com/user-attachments/assets/f4206463-5d3f-4d2f-8ac9-72de18a1268d" />


Linux Colors:
------------
R -> 31
G -> 32
Y -> 33

echo -e "\e[31m Hello \e[33m World"

Hello in Red
World in Yellow

<img width="577" height="97" alt="image" src="https://github.com/user-attachments/assets/a153216c-e625-4399-a8bd-2f4cccb9f3a4" />


Error Handling:
---------------
1. Expected Errors
2. Unexpected Errors

   Set -e
   ---------
<img width="242" height="173" alt="image" src="https://github.com/user-attachments/assets/61376eb3-3ec9-47da-842f-24ac5a9cdcb8" />

<img width="567" height="61" alt="image" src="https://github.com/user-attachments/assets/bb1adc42-91d9-44b6-9bec-1957a2654c1d" />

on putting -> set -e , the control stops once the script encounters errors.


 Trap Command:

 <img width="574" height="458" alt="image" src="https://github.com/user-attachments/assets/66aa825d-5e14-4173-8813-ec808522111f" />

<img width="577" height="65" alt="image" src="https://github.com/user-attachments/assets/306f84b6-7588-4b5d-8a8c-4e07ac1d4ff8" />









