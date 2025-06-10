# Linux-Agency_tryhackme_walkthrough
This Room will help you to sharpen your Linux Skills and help you to learn basic privilege escalation in a HITMAN theme. So, pack your briefcase and grab your SilverBallers as its gonna be a tough ride.

Welcome to Linux Agency. Agent 47, this is where you will need to go through several tests concerning linux fundamentals and privilege escalation techniques.
This room is proudly made by 0z09e and Xyan1d3
If you enjoy this room, please let us know by tagging us on Twitter. You may also contact us in case of some unintended routes or bugs, and we will be happy to resolve them.

## Task - 1 :
Deploy the machine.

## Task - 2 : 
Please wait about 1 minute before SSH’ing into the box.

**SSH Username : agent47**

**SSH Password : 640509040147**

Each flag found will serve as the password for the next user. The flag includes the username of the next user that is part of this challenge. The Flag format is : username{md5sum}
The order of users: agent47 --> mission1 --> mission30 will be part of Task 3: Linux Fundamentals.
After those missions, the next levels will be in Task 4: Privilege Escalation.

SSH into the box as agent47

## Task - 3 :
Agent 47, we are ICA, the Linux Agency. We will test your Linux Fundamentals. 

Let's see if you can pass all these challenges of basic Linux. 

The password of the next mission will be the flag of that mission. Example: mission1{1234567890} will be the password for the mission1 user.

**Mission 1**

Login to mission1 user to get mission2 flag. 

### Command - su mission1 ###

![1_LSN9zygf4ScR5fxGNo3ogg](https://github.com/user-attachments/assets/cf499da4-9a7a-4f8a-812c-94e5534e76fc)

**Mission2**

By changing to the home directory of mission1 user, we find the flag of mission2

![image](https://github.com/user-attachments/assets/dddc69a6-30d1-4e8b-99ec-9567fe044f01)

**Mission3**

By changing to the home directory of mission2 user, we find the flag.txt.

By using cat command we can read the flag.txt file.

![image](https://github.com/user-attachments/assets/fc60b97e-4171-422a-bca0-98865842346e)

**Mission4**

By changing to the home directory of mission3 user, we find the flag.txt.

Unfortunately, this time we cannot find the flag by using cat command.

So, we replace cat command by strings and check whether if it works.

![image](https://github.com/user-attachments/assets/044567b9-4eeb-45d8-8cea-50e207c1d504)

**Mission5**

By changing to the home directory of mission4 user, we find the flag.txt.

![image](https://github.com/user-attachments/assets/ad247ad5-11dd-4f16-99c2-db9b3ccc7c3a)

**Mission6**

By changing to the home directory of mission5 user, we find the flag.txt.

![image](https://github.com/user-attachments/assets/979b8f54-9988-4f81-be2f-f90ca5f52c38)

**Mission7**

By changing to the home directory of mission6 user, we find the flag.txt.

![image](https://github.com/user-attachments/assets/1bddf203-0afb-4ed7-8818-5c22c1239d77)

**Mission8**

Since we change to mission7 user there is a suspicious “Permission denied” message.

Changing to current user’s home folder specifying the path (cd /home/mission7 or cd ../mission7) should solve the issue.

![image](https://github.com/user-attachments/assets/59ed698c-98b8-4a97-b33a-9b33c7f62b4d)

**Mission9**

By switching to mission8 user we cannot find flag.txt.

Well, we can try to search for it in all the system.

![image](https://github.com/user-attachments/assets/6fd6c4e8-c41d-421a-801e-42d89f3747e1)

**Mission10**


