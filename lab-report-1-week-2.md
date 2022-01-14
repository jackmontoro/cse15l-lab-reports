
# Lab1 Report
The objective here is to:
* Get familiar with VSCode and ssh
* Feel confident using the VSCode IDE


To this end we will:
1. Introduce ourselves to the group
2. Post a screenshot of our VSCode homepage to demonstrate that it is working
3. Access ieng6 remotely through ssh and post a screenshot


Before we get started, you will need to change your password for the student account related to this course in order to make to best use of your time. The system will take around 5-15 minutes to update your password, so it is good to do this as soon as possible. You can access your account by following the link below.

[course-specific account](https://sdacs.ucsd.edu/~icc/index.php)

Once you update your password for this course, you can log onto UCSD's remote servers to access its files. We do this through a terminal command called ssh, but we will get to that later.

You must first install Visual Studio code to your computer:

[vscode setup](https://code.visualstudio.com/)

There will be instructions on installation once you get to the VSCode download webpage.
 
Once installed the environment will look something like this, but you will probably see a welcome message:
![VSCode Screenshot](Lab2Screenshot.png)

When you have VSCode up and running, you can log into the ieng6 remote serve using the following ssh command:

> $ ssh cs15lwi22zz@ieng6.ucsd.edu

The terminal will ask you for your password that you set up on your course account, so type that in and press enter. As stated previously, your password info could take up to 15 minutes to update from the time you changed it.

Once you enter your password, your output should look like this:
![ssh](sshScreenshot.png)

Now, you can run some commands! Here are a few you can try:

* cd  This one allows you to move between directories so you can access files.
* ls  This will provide you with a list of the files within the directory you are currently in
* ls -lat
* ls -a
* cp /home/linux/ieng6/cs15lwi22/public/hello.txt ~/
* cat /home/linux/ieng6/cs15lwi22/public/hello.txt

Once you are done experimenting with commands, you will need to log out of the remote server.
To do this you can use the Ctrl+D hotkey or run the following command:
> exit

In the top-left corner of your screen click File->New File to create a new file which you will name `WhereAmI.java`. Once creater, you will post the following code:
 
```
 class WhereAmI {
  public static void main(String[] args) {
    System.out.println(System.getProperty("os.name"));
    System.out.println(System.getProperty("user.name"));
    System.out.println(System.getProperty("user.home"));
    System.out.println(System.getProperty("user.dir"));
  }
 }
 ```
 From the directory where you made this file, you will type the following command from the terminal:
 ```
 scp WhereAmI.java cs15lwi22zz@ieng6.ucsd.edu:~/
 ```
 




