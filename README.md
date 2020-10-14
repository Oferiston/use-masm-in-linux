# Steps to Do
## install dosbox in your system
use your own package manager command with sudo privilige to install dosbox like:

**sudo zypper in dosbox**

while **sudo** ask for sudo privilige which is required in most of the occasions. **zypper** is the package manager name for openSUSE(a linux version made by German). **in** means install for zypper and **dosbox** is the package name. Notice sometimes the package name is different from its usual software name so the best way before the installation of a package is to search the software's package name in different distributions. You can search it in any engines you like or use command like this:

**sudo zypper search dosbox**

It returns a chart including all packages whose name includes dosbox such as dosbox-sid and uninsdosboxoio-siodi.

## run dosbox in your directory
You could run dosbox by clicking its icon in the search bar or application bar but more efficiently you could directly type **dosbox** in the bash and the window will show up. Focus on the dosbox's command line, it may start with **Z:>**, or anything else. You may need to redirect the directory to somewhere on your computer to make dosbox be able to use files you made. Command is :

**mount c ~/pathOne/pathTwo**

Here c is the symbol. Best choice is c. ~/pathOne/pathTwo is the directory name. Here ~ represents /home/yourUserName. You could input absolute path too which is recommended.

To use a new shell system, first type Help or HELP or anything else to ask for directions. You could learn some basic use in dosbox through doing so like dir to list all files and directories and cd to switch directories. Or you could search mannual or tutorials online for help.

Now if you input the command above (**mount c ~/pathOne/pathTwo**) , you see nothing happened, if its **Z:>** before, it still didnt change. Du~de, we need one more step. Remember we use **c** after mount. We may type command below in the dosbox shell:

**c:**

and after this you would see the letter finally changed. dir it and you could see the files in your input directory be listed below.

##  excute exe in dosbox
Dosbox actually is a simulator for a specific environment which means the dosbox file system could be very different from your linux file system. For example .exe file can't directly be executed in linux while it can be done in dosbox. 

We did set a path on our computer for dosbox to use earlier. The directory we set for dosbox is a platform where dosbox can read files and do its own stuff. Since .exe files can't be excuted by linux but can be executed in dosbox, we put .exe files in the directory we set for dosbox. And type the name of the .exe file, we can see it be run or executed in dosbox.

## assembeler tools
But we need dosbox just for enviroment simulation. What should we do if we need to assemble .asm files? 

Well you could use nasm in linux which is recommended. Just install nasm using command we use to install dosbox above, don't need to search, the package name is nasm itself. 

But some people would still need masm. If we need to assemble .asm in Intel 80 86 chips (8086,8088,80286,80386,80486 and pentium. These chips have some differences on the CPU registers' bits number and names. Further information may require an assembly language tutorial book) environment, we need masm to do this step. 

What's masm? masm is a .exe file with a full name Microsoft Macro Assembler from where we can see why it's .exe file. How to use masm in linux? Like what we analyzed, we need to move masm.exe in the directory we set for dosbox, type masm and let dosbox execute the masm.exe file. 

Well we did it! One more stuff is that assembling .asm files not only needs masm, but also needs many other tools which are all .exe files. We obey the same way we do for masm.exe. And the directory we set for dosbox can now be called as an assemble enviroment. If we wanna do any assembling work, make .asm files in pure text format in that directory and use tools(masm and etc) in the dosbox shell, we will get the result. The normal procedure to use these tools are: masm fileName, link fileName, fileName.

For example we created and wrote sample.asm in the directory we set for dosbox. Now we do:

**masm sample;**  make sample.obj file

**link sample;** make sample.exe file through sample.obj 

**sample** execute sample.exe like execute masm.exe by just typing masm

We will see the result be displayed on the dosbox (0,0,0) screen with (255,255,255) frontface color. Notice ; at the end of masm and link command means jumping all other questions.

## masm and other tools file
Well now we need only the tools' files, of course .exe type. You can download them online using all the ways. Here are these tools provided in the tools folder.
