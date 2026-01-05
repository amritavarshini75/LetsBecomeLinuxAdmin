Process management commands

kill -9 pid - this will stop the process fully
kill -3 pid - in case a developer asks you for a thread dump for a particular process then you use this command to safely 
take the thread dump and provide the developer process threads oriented data which helps them to figure out which function or which code is taking up more space, cpu utilization stats and much more.
kill -STOP pid - this command is used to temporarily suspend a process on the server
