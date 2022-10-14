![Image]([https://github.com/sylvanabrooke/cse15l-lab-reports/blob/8b958fff6301dc131950d35de409c07a49a5f337/Screen%20Shot%202022-09-30%20at%205.56.58%20PM.png](https://github.com/sylvanabrooke/cse15l-lab-reports/blob/8b958fff6301dc131950d35de409c07a49a5f337/Screen%20Shot%202022-09-30%20at%205.56.58%20PM.png?raw=true))
* google vscode from a web browser
* download vscode
* open it on your computer

![Image]([https://github.com/sylvanabrooke/cse15l-lab-reports/blob/7f2906dd104ad4339d12e7a3c0a318c508682ace/Screen%20Shot%202022-09-30%20at%204.31.22%20PM.png](https://github.com/sylvanabrooke/cse15l-lab-reports/blob/7f2906dd104ad4339d12e7a3c0a318c508682ace/Screen%20Shot%202022-09-30%20at%204.31.22%20PM.png?raw=true))
* make sure ssh is downloaded onto vscode, then open "Remote-SSH: Connect to Host..." from the command palatte
* type in your username and @ieng6.ucsd.edu to open your server
* type in your password when prompted- it won't show characters, but it is being typed, and hit enter

![Image]([https://github.com/sylvanabrooke/cse15l-lab-reports/blob/107b050553c773e930d3bf1af2b0dfa697a0578a/Screen%20Shot%202022-09-30%20at%204.41.26%20PM.png](https://github.com/sylvanabrooke/cse15l-lab-reports/blob/107b050553c773e930d3bf1af2b0dfa697a0578a/Screen%20Shot%202022-09-30%20at%204.41.26%20PM.png?raw=true))
* try some commands, such as cd, ls, pwd, mkdir, and cp on your computer, and the server
* you can see the list of files in the server by typing ls-a

![Image]([https://github.com/sylvanabrooke/cse15l-lab-reports/blob/0846a19a311616d3fcd9ef7b9d5617ac37ed6070/Screen%20Shot%202022-09-30%20at%204.41.01%20PM.png](https://github.com/sylvanabrooke/cse15l-lab-reports/blob/0846a19a311616d3fcd9ef7b9d5617ac37ed6070/Screen%20Shot%202022-09-30%20at%204.41.01%20PM.png?raw=true))
* Make a file on your own computer
* run it with scp in front and your username on the end, like this: scp WhereAmI.java cs15lfa22zz@ieng6.ucsd.edu:~/
* you can now run it on the server's terminal

![Image]([https://github.com/sylvanabrooke/cse15l-lab-reports/blob/1f7a67b23782a6d7b3ec2698c75332d6314ff267/Screen%20Shot%202022-09-30%20at%206.17.03%20PM.png](https://github.com/sylvanabrooke/cse15l-lab-reports/blob/1f7a67b23782a6d7b3ec2698c75332d6314ff267/Screen%20Shot%202022-09-30%20at%206.17.03%20PM.png?raw=true))
* to make a key, ensuring that you don't have to put your password in when switching between servers: type ssh-keygen
* type enter until it makes a visual key, then type ssh cs15lfa22zz@ieng6.ucsd.edu
* in your server, type mkdir .ssh, then log out and type scp /Users/<personal username>/.ssh/id_rsa.pub <ucsd username>@ieng6.ucsd.edu:~/.ssh/authorized_keys
![Image]([https://github.com/sylvanabrooke/cse15l-lab-reports/blob/9e6c92d46c0cbe6ecaa5cdeb5efeb2e99375e90a/Screen%20Shot%202022-09-30%20at%206.21.31%20PM.png](https://github.com/sylvanabrooke/cse15l-lab-reports/blob/9e6c92d46c0cbe6ecaa5cdeb5efeb2e99375e90a/Screen%20Shot%202022-09-30%20at%206.21.31%20PM.png?raw=true))
* you can simplify commands by putting them in quotes, ex: ssh cs15lfa22@ieng6.ucsd.edu "ls"
* you can also use semicolons to run multiple commands on one line, ex: cp WhereAmI.java OtherMain.java; javac OtherMain.java; java WhereAmI
