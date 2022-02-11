#Lab Report 3

For my option, I elected to copy one of my repositories to a remote server via scp -r. I chose my repository markdownparse-jackweek5 to copy to the server. I input the following code to the terminal: 

```scp -r . cs15lwi22abf@ieng6.ucsd.edu:markdownparse-jackweek5```

After ssh-ing into my student server, I found that the repository had been copied to the server.

![image](scpResult.png)


After copying the entire repository to the remote server, I used ssh to log on and ``cd`` to get to my ```markdownparse-jackweek5``` repository.
Once I moved to my repository, I used the command ```make test``` to compile and run my tests and generate class files.

![image](makeTest)