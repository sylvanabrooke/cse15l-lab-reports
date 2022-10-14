![Image](image1./image.png)
* google vscode from a web browser
* download vscode
* open it on your computer

![Image](image2./image.png)
* make sure ssh is downloaded onto vscode, then open "Remote-SSH: Connect to Host..." from the command palatte
* in terminal type in "ssh" + your username + @ieng6.ucsd.edu to open your server
* type in your password when prompted- it won't show characters, but it is being typed, and hit enter

![Image](image3./image.png)
* try some commands, such as cd, ls, pwd, mkdir, and cp on your computer, and the server
* you can see the list of files in the server by typing ls-a

![Image](image4./image.png)
* Make a file on your own computer
* run it with scp in front and your username on the end, like this: scp WhereAmI.java cs15lfa22zz@ieng6.ucsd.edu:~/
* you can now run it on the server's terminal

![Image](image5./image.png)
* to make a key, ensuring that you don't have to put your password in when switching between servers: type ssh-keygen
* type enter until it makes a visual key, then type ssh cs15lfa22zz@ieng6.ucsd.edu
* in your server, type mkdir .ssh, then log out and type scp /Users/<personal username>/.ssh/id_rsa.pub <ucsd username>@ieng6.ucsd.edu:~/.ssh/authorized_keys
  
![Image](image6./image.png)
* you can simplify commands by putting them in quotes, ex: ssh cs15lfa22@ieng6.ucsd.edu "ls"
* you can also use semicolons to run multiple commands on one line, ex: cp WhereAmI.java OtherMain.java; javac OtherMain.java; java WhereAmI
