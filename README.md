Download Link: https://assignmentchef.com/product/solved-cpsc1021-lab-1-hello-linux
<br>
During this lab you will:

<ol>

 <li>Login into the department Linux machines;</li>

 <li>Practice using the command line interface;</li>

 <li>Type, compile and run a small C++ program;</li>

 <li>Create a zipped archive called “tarball”, and submit it to canvas.</li>

</ol>




<h1>Part I – Logging into Linux</h1>

To login into Linux you need your Clemson University username and password. Type them into the login boxes, and you are in!!! Now take a look around.

Linux is an operating system much like Windows and MacOS. An operating system’s job, broadly speaking, is to allow software applications to access hardware resources like the CPU and storage disks. Unlike proprietary operating systems (again, Windows/MacOS), Linux is notable in that it is open sourced and free!

Open source software is maintained and developed by the community at large, which means Linux was written by programmers for programmers. There are many flavors of Linux with varying degrees of user friendliness. In this lab we will use Ubuntu Linux, that has emerged as a great general-purpose OS.

Using your favorite search engine, please find out what the name “Ubuntu” means,                  and what language it comes from. Discuss your findings with the TAs.

Similar to Windows and MacOS operating systems, Linux has a graphical user interface (GUI, pronounced as “goo-ee”). But the real power of Linux is in its command line utility which allows users to quickly and efficiently type commands at the prompt without the distraction of the graphical elements. This is what we will use today and in the future labs.




<h1>Part II. Using command line interface</h1>

<h2>Creating directories</h2>

<ol>

 <li>Right-click on the desktop and select Terminal. This will open a terminal window where you will type different commands. The terminal will usually open to your <em>home directory</em>.</li>

</ol>




<ol start="2">

 <li>Enter the <em>pwd</em> (“print working directory”). The working directory should be /home/<em>your_username</em>. This is known as your <em>home directory</em>. All your files and directories will be kept in a directory tree with this directory as root.</li>

</ol>




<ol start="3">

 <li>Enter <em>mkdir 1021labs </em>to create a directory named 1021labs for your labs this semester.</li>

</ol>




<ol start="4">

 <li>Enter <em>ls</em> to list the contents of the current directory. You should see the new <em>1021labs</em></li>

</ol>




<ol start="5">

 <li>Now you need to move into that directory. Enter <em>cd 1021labs </em>to change the working directory.</li>

</ol>




<ol start="6">

 <li>Enter <em>mkdir lab1 </em>to create a folder for today’s lab.</li>

</ol>




<ol start="7">

 <li>Enter <em>mkdir temp </em>to create a temporary directory. (you will learn how to remove this directory in a few minutes)</li>

</ol>




<h2>Using terminal editors to write code</h2>

<strong><em> </em></strong>

<ol>

 <li>There are several editors that you can use while writing code in the terminal. The easiest to use is <em>pico</em>. You can open it by typing <em>pico</em> on the command line. When it opens, you will see a window with a number of command abbreviations on the bottom. Press <em>Ctrl</em> and <em>O </em>(Overwrite means save) and give your file a name. Save your work very often, so you do not lose it! It does not take long to press <em>Ctrl</em> and <em>O</em> keys ans may save you a lot of headache later. To exit <em>pico</em> press Ctrl and <em>X</em> (X is for exit). There are also other options that you can explore on your own. This editor is very simple to use, though it does not have a lot of useful extensions.</li>

</ol>




<ol start="2">

 <li>Not all systems come with<em> pico</em>, but all of them come with <em>vim</em>. <em>vim</em> is a very powerful editor, but it does require a short learning curve to learn all the shortcuts. Knowing how to use vim is a valuable skill that each programmer should have. Next labs will be done using <em>vim</em>. In case you want to try <em>vim</em> today, here is a link with the beginner’s guide: <a href="https://www.linux.com/tutorials/vim-101-beginners-guide-vim/">https://www.linux.com/tutorials/vim</a><a href="https://www.linux.com/tutorials/vim-101-beginners-guide-vim/">–</a><a href="https://www.linux.com/tutorials/vim-101-beginners-guide-vim/">101</a><a href="https://www.linux.com/tutorials/vim-101-beginners-guide-vim/">–</a><a href="https://www.linux.com/tutorials/vim-101-beginners-guide-vim/">beginners</a><a href="https://www.linux.com/tutorials/vim-101-beginners-guide-vim/">–</a><a href="https://www.linux.com/tutorials/vim-101-beginners-guide-vim/">guide</a><a href="https://www.linux.com/tutorials/vim-101-beginners-guide-vim/">–</a><a href="https://www.linux.com/tutorials/vim-101-beginners-guide-vim/">vim/</a><a href="https://www.linux.com/tutorials/vim-101-beginners-guide-vim/">.</a> You can also google vim tutorials and youtube videos.</li>

</ol>




<ol start="3">

 <li>Alternatively, if you are familiar with Linux and already have your own favorite editor, you can use that editor today.</li>

</ol>







<h2>Using other commands</h2>

With the help of your TAs please practice using other commands:               cp <em>file1 file2</em>  copies file named <em>file1</em> into a file named <em>file2</em>.            rm file1  deletes <em>file1.</em>          mv <em>file1 file2</em>  renames <em>file1</em> to <em>file2. </em>

ls  lists files and directories in the current directory         cd ..  changes to a directory one level up.          cd ~ changes to your home directory.      clear  clears the screen.




<h2>Getting additional help with Linux commands</h2>

Occasionally you will have questions about how a Linux command is used. There is no programmer who knows or remembers everything. It is very important that you can help yourself to find the necessary information. You have a couple of options here.

<ol>

 <li>You can type the name of the command you need help with, followed by “–help”, that is, two minus signs and the word <em>help</em> without spaces between them. For example, to know more about the command <em>cp</em>, you would type this at the prompt:</li>

</ol>




cp  –help  |  less

The | (“pipe”) character and the word <em>less </em>after the command have a special purpose. The output of the command “cp –help” is “piped” or redirected into another command (<em>less</em>). <em>Less</em> is a Linux utility that formats the help entry so that if the entry is too long, you can see one screen at a time. It allows you to scroll up and down. To exit the help mode, press the <em>q </em>key on the keyboard. Try and run the command “cp –help” with and without the “| less” and observe the differences.

<ol start="2">

 <li>Another useful option is the online system manual, or <em>man</em>. Every Linux system comes with online documentation that explains how the system commands and utilities are to be used, and what options they have. To use the online manual to lookup a command, you would type:</li>

</ol>




man cp  |  less

As above, you will pipe your command into the <em>less</em> to be able to see information one screen at a time.




Now go ahead and practice using <em>man</em>. Look up such commands as less, more, cat, date, calendar, and clear. What happens if you type <em>man man</em> ?




<ol start="3">

 <li>Being able to use a search engine is also a good idea. Every time you come across something you do not know, you can help yourself right away by looking it up online. There is so much information out there waiting to be discovered! And the good news is, you already know how to look information up online.</li>

</ol>







<strong>Part III. Creating a simple C++ file, compiling and running it.  </strong>

<strong> </strong>

<ol>

 <li>Using an editor of your choice, create a file named <em>cpp</em>. C++ files need to have an extension .cpp to let the compiler know that this is a C++ file. Type a small program that produces the output shown below. You can see examples in Chapter 2 of your textbook. Your output should be printed exactly as shown below, on two lines.</li>

</ol>




This is my first C++ program !

I love Linux !




<ol start="2">

 <li>Compile your program. The name of the compiler we will use is g++. Your executable file should be named <em>out</em>. To do this you will type the following command:</li>

</ol>




g++ lab1.cpp -o lab1.out




By default compiler would create an executable file named <em>a.out</em>. If we want to name our executable differently (for example, <em>lab1.out</em>), we need to specify this with the option “-o” at compile time.




Why wouldn’t we just leave the default name <em>a.out</em>?  Imagine you have a number of files in the same directory, and you want to compile them all and keep their executables in the same directory. You cannot! Every time you compile a file, the newly generated <em>a.out</em> will overwrite the previously created one!




Tu run your program just type <strong>./lab1.out</strong>, and you should see your output on the screen. If the output does not look like the one shown above, please go back and correct your code. Recompile and rerun.







<strong>Part IV. Creating a “tarball”. </strong>




Before you do the next step, you need to backup the file you just created. Backing up a file means to create a copy of it in another location, so that if something went wrong, or you have accidentally deleted or corrupted your file, you still have a backup copy.




It is often necessary to create a zipped archive that contains several files. This is similar to zipping files on a Windows machine to create one .zip file. On a Linux machine this is called

“creating a tarball”, since the utility used to create it is called “tar”, an abbreviation for “tape archiver”. On older machines many years ago files were archived on a tape, and that name is still used for this useful utility. In this lab we will create a tarball with only one file in it – the C++ file you have created in the step above. The syntax of the command to create an archive is below:

tar cvf <em>file.tar dir</em>




The options “cvf” tell the <em>tar</em> utility what to do, for example, <em>c</em> means create an archive, <em>v</em> means do it in a verbose mode, <em>f</em> means file.  <em>file.tar</em> is the name of your archive, it should have an extension “.tar”, and <em>dir</em> is the directory or the file you would like to archive.




<strong>NOTE:</strong> there is a possibility to corrupt/delete your work files if you do not use the command correctly. The name of the tar file should precede the name of the file/directory to archive.




After you have created an archive, you will use another utility to compress it.

gzip file.tar




This will compress the archive and now you will see an extension.gz added to the filename: <em>file.tar.gz. </em>

<strong> </strong>

<h2>Extracting files from the tarball</h2>

To extract the files from the tarball you will have to unzip the file first by using the command:




gunzip file.tar.gz




This will unzip the archive and remove the extension .gz from the filename. Next you will extract files from the archive:

tar xvf file.tar




The option <em>x</em> means you are extracting files. Occasionally, you will want to examine the contents of the archive without actually extracting the files. You can do this with the following command.

tar tvf file.tar




<em>t</em> here is used to list the contents of the archive.




At this point you need to practice creating a zipped archive and extracting files from it. Make sure you have backed up your C++ file first, just in case.