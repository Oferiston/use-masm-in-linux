# Steps to Do
## install dosbox in your system
use your own package manager command with sudo privilige to install dosbox like:

**sudo zypper in dosbox**

while zypper is the package manager name for openSUSE(a linux version made by Germans). **sudo** ask for sudo privilige which is required in most of the occasions. **in** means install for zypper and **dosbox** is the package name. Notice sometimes the package name is different from its usual software name so the best way is to search the software's package name in different distributions. You can search it in any engines you like or use command like this:

**sudo zypper search dosbox**

It returns a chart including all packages whose name includes dosbox such as dosbox-sid and uninsdosboxoio-siodi.

## run dosbox in your directory
You could run dosbox both click its icon in the search bar or application bar but more efficiently you could directly type **dosbox** in the bash and the window will show up. Focus on the command line, it may start with **Z:>**, or anything else. You need redirect the directory to somewhere on your computer. Command is :

**mount c ~/pathOne/pathTwo**

Here c is the symbol, best choice is c. ~/pathOne/pathTwo is the directory. Here ~ represents /home/yourUserName. You could input absolute path too which is recommended.

To use a new shell system, first type Help or HELP or anything else to ask for directions. You could learn some basic use in dosbox doing so like dir to list all files and directories and cd to switch directories. Or you could search mannual or tutorial online for help.

Now if you input the command above and you see nothing happened, if its **Z:>** before it didnt change. Du~de, we need one more step. Remember we use **c** after mount. We type command below in the dosbox shell:

**c:**

and after this you would see the letter finally changed. dir it and you could see the files in your input directory listed below.

##  excute exe in dosbox
Dosbox actually is a simulator for a specific environment which means the dosbox file system could be very different from your linux system. For example .exe file cant directly excute in linux while it can be done in dosbox. 

We did set a path on our computer in dosbox earlier. The directory we set for dosbox is a platform where dosbox can read files and do its own stuff. Since .exe files cant be excuted by linux but can be executed by dosbox, we put .exe files in the directory we set for dosbox. And type the name of the .exe file, we can see it run or executed in dosbox.

## assembeler tools
But we need dosbox just for enviroment simulation. What should we do if we need to assemble .asm files? 

Well you could use nasm in linux which is recommended. Just install nasm using command we use to install dosbox above, dont need to search, the package name is nasm itself. 

But some people would still need masm. If we need to asseemble .asm in Intel 80 86 chips (8086,8088,80286,80386,80486 and pentium) environment, we need masm to do this step. 

What's masm? masm is a .exe file. How to use masm in linux? Like what we analyzed, we need to move masm.exe in the directory set for dosbox, type masm and let dosbox to execute the .exe file. 

Well we did it! One more stuff is assemble .asm files not only needs masm, but also needs many other tools which are all .exe files. We obey the same way we do for masm. And the directory we set for dosbox can now be called as an assemble enviroment. If we wanna do any assembling work, make .asm files in that directory and use tools(masm and etc) in the dosbox shell, we will get the result.

## masm and other tools file
Well now we need only the tools' files, of course .exe type. You can download them online using all the ways. Here are these tools provided in the tools folder.
