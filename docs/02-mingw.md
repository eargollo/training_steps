# Installing Git for Windows

## First install Chocolatey

Chocolatey is a package manager for Windows and it will help you install most of the needed tools for this training.

Go to https://chocolatey.org/ and follow the steps to install Chocolatey.

## Install Git for Windows

Use choco to list for the msysgit package:

```bash
C:\windows\system32>choco list msysgit
Chocolatey v0.10.8
git.install 2.15.1.2 [Approved]
git 2.15.1.2 [Approved]
msysgit 1.7.10.20120526 [Approved]
Cmder 1.3.3 [Approved] Downloads cached for licensed users
git.portable 2.15.1.2 [Approved]
kellyelton.devenvironment 1.0.0.11 - Possibly broken
Devbox-Git 1.8.1.20130422 - Possibly broken
cmdermini 1.3.3 [Approved] Downloads cached for licensed users
8 packages found.
```

Install the msysgit package:

```bash
C:\windows\system32>choco install -y msysgit
```

Once the package is installed you will be able to execute the MSysGit terminal (Git Bash).

Explore a bit the terminal. Note that the `\` is different than Windows.

Run the `pwd` command and check the result. It tells you at what path you are. Note that the `C:` maps to `/c`.

Run the `ls` command to see the contents of the current folder. Check the `ls -la` command. 

Mind that any folder started with `.` will not be shown at `ls` but will show at the `ls -la`.

If you still have some time explore which common commands from linux are available at MINGW terminal. Check some commands at [10 commands](http://www.informit.com/blogs/blog.aspx?uk=The-10-Most-Important-Linux-Commands)

Check shortcuts (I really like the Ctrl+R and arrows) and system info [here](https://community.linuxmint.com/tutorial/view/244).

If you are still having fun, search in Google for the Grep command. It will be very useful down the road. Take also a look at linux pipe `|`.

Try this command and see if you can understand it:

```
find | grep exe
```

What about this:

```
grep step * -r
```
