# Monitoring Commands

## 1. top command 
```bash
top
````
* The monitoring commands are also usually related to the process management. Usually ps aux | grep <process_name> will give you so many processes in real time. So if you want to know top memory/cpu consuming process based on real time data we use top command. It lists all the processes in descending order of cpu/memory utilization.
* It also dynamically keeps changing the list accordingly.

<img width="950" height="341" alt="image" src="https://github.com/user-attachments/assets/da7f20fe-03e5-46da-bdac-d18c8d9fa545" />

*The enhanced version of top is the htop. It does not come inbuilt on thr linux server. You can install using yum install htop. It gives you a better visualization of the top command output and easier to interpret the information as well.

```bash
htop
````

<img width="959" height="332" alt="image" src="https://github.com/user-attachments/assets/5a4c3236-7e15-4719-9331-5f47abe4a3c6" />
