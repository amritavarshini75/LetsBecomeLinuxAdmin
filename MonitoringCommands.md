# Monitoring Commands

## 1. top command 
```bash
top
````
* The monitoring commands are also usually related to the process management. Usually ps aux | grep <process_name> will give you so many processes in real time. So if you want to know top memory/cpu consuming process based on real time data we use top command. It lists all the processes in descending order of cpu/memory utilization.
* It also dynamically keeps changing the list accordingly.

<img width="950" height="341" alt="image" src="https://github.com/user-attachments/assets/da7f20fe-03e5-46da-bdac-d18c8d9fa545" />

* The enhanced version of top is the htop. It does not come inbuilt on thr linux server. You can install using yum install htop. It gives you a better visualization of the top command output and easier to interpret the information as well.

```bash
htop
````

<img width="959" height="332" alt="image" src="https://github.com/user-attachments/assets/5a4c3236-7e15-4719-9331-5f47abe4a3c6" />

## 2. vmstat command 

```bash
vmstat
````
* The vmstat command is useful for checking the linux server or system performance.
* Lets consider this scenario - suppose if anyone comes and complains that the ec2 instance or the vm is slow. Then to verify its performance we opt for vmstat command
<img width="550" height="56" alt="image" src="https://github.com/user-attachments/assets/221b680c-eac8-4d01-91e8-39247e893157" />
* If you observe the above mentioned image, if free memory is more then it indicates that system is functioning normally. Also make sure that the cache memory is not too high
* Now incase you want to just check how much free space is present on the server you can opt for free -m / free -h command.
```bash
free -m
free -h
````
* The -h option gives the command output in a human readable format so that you can easily understand how much mb of disk is free and all.
<img width="554" height="50" alt="image" src="https://github.com/user-attachments/assets/2f596064-2c95-45d4-aa43-fbf987e0cbd7" />
<img width="548" height="53" alt="image" src="https://github.com/user-attachments/assets/0ec2e3e4-5a51-4900-b559-c705401ca088" />

## 3. nproc command
* This command will give you the number of cpus available on the machine
```bash
nproc
````
<img width="221" height="28" alt="image" src="https://github.com/user-attachments/assets/f22b966d-f342-43a5-a6a8-cec8f8d4028b" />





