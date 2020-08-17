---
layout: post
title: Termux - The android Terminal
---

No hesitation, you can certainly call Termux "The Android terminal". Owing to it's simplicity and capabilities, Termux stand so close to the original Linux terminal.

### Who is it for and who should read this?
This is beginner article which will introduce you to the fundamentals of using Linux terminal on android devices. To understand something here, you should barely understand English and nothing else is a pre-requisite. &#129299;


### Let us figure out the basics.
#### Android
If you are using an android device, you know that android is the operating system that run the show on your mobile phone.
Android is an operating system with its core based on Linux. In fact, android is based on a modified version of Linux optimized for mobile devices.

#### Terminal
Terminal is a command line interface which can be used to communicate with or control the Operating system. So, a linux terminal can be used to control a Linux device. Terminal is a tool that comes default with a full fat Unix or Linux oprating system. Terminal helps the users do a lot of things by running the commands.
By default, android does not enable the Terminal for the regular users. That means, we cannot get a terminal on android device out of the box. 

#### Termux, the star of the show
Termux is an application that can be downloaded from Play store. Termux is a terminal emulator. Emulator is nothing but a system that does a sort of simulation of something on top of another system. In this context, the Termux will act as a Linux Terminal on top of the Android operating system.

#### Let us get it.
We can download and install Termux app from Google Play. This is a clean app and there is no shady business here. &#9996;
For the lazy ones, it is just a [ click ](https://play.google.com/store/apps/details?id=com.termux) away. &#128521;

### The look and feel of the Terminal( rather, Termux)
After installing Termux, upon opening , it shows up with a black screen and white letters.The crowd familiar with the DOS command line or Linux terminal will feel at home for sure.

<img src="/images/posts/Termux1/TermuxHome.jpg" alt="Termux home" width="270" height="500" class="center">

### Some upgrades
The programs and the installed packages will be updated by the corresponding developers from time to time. The updates are nothing but new features, bug fixes or some improvements. We should also try to keep our system upto date by installing the updates. 
It is easy to run two commands to keep your system updated.

```
#This is how we add some comments
apt update


```
After the above command is executed, you can see any available updates for your installed packages.

<img src="/images/posts/Termux1/TermuxUpdate.jpg" alt="Termux Update" width="270" height="500" class="center">

Now we have to install the available packages. To install the available packages, just run the command given below. It will prompt you for the confirmation to install. Please input Y or y.
```
apt upgrade

```
<img src="/images/posts/Termux1/TermuxUpgrade.jpg" alt="Termux Upgrade" width="270" height="500" class="center">


Good, we are all set. Now we can look for having some fun.

### Running some custom programs

We have a working Terminal now, thanks to Termux. We can run custom programs on your android device. The easy way to do something is to run some applications already available on github.

#### Github
Github is a free public reposity available at https://github.com/. You can create a free account, save and share your code or applicatons with other developers. You can access the repostories which are made available to the public by other developers. It is a fantastic collaboration tool and doesn't cost you a penny.

#### Getting the public code or applications from Github

1. Create an github account.
  This is a no brainer activity. Nobody need any assistance here.
2. Install git on Termux.
  To install git on Termux, run the following command on the Termux terminal.
```
pkg install git
```
<img src="/images/posts/Termux1/TermuxGitInstall.jpg" alt="Termux Git Installation" width="270" height="120" class="center">
3. Checkout or clone the code from github to your phone.

I am going to use a Github repo called "ShellScripts" owned by the developer "RapidSailor". This is by far the simplest shell script repo you can get.
It is a one line command to copy the code to your local phone storage.

```
#The below command will copy the code from the given repo to your phone.
git clone https://github.com/RapidSailor/ShellScripts

```
#### Inspect downloaded code

When you run the above command , the repo is copied to your current woring folder on your phone.
To see what all files are there , run the below commands.
The below command will list all the repos which you have copied to the phone. right now, it will be only one.
```
ls
#Navigate into the downloaded repo
cd ShellScripts
#check the contents in the downloaded repo
ls

```
You can see that this repo has only one file - 'echo.sh' .

#### Making the file executabe
We have only one file that can be executed. To execute any file in Linux, the file should have the 'Execute' permission.
Running one command will make a file executable.

This command 'chmod' is used to change the mode. Tha parameters '+x' indicate the execute permission to the training file names.

```
chmod +x echo.sh
#
```
Now the file is executable. &#128526;

#### Run the application &#128513;
Running an executable file is another single command.
since this program is an shell script, we run the below command.

```
sh echo.sh
```
Now the program will execute and display any outcome as needed.
The screenshot below with show the sequence of execution and its outcome.

<img src="/images/posts/Termux1/TermuxExecute.jpg" alt="Termux Execution" width="270" height="250" class="center">

We are done executing a basic shell script program using Termux on your android phone. &#128519;

Doesn't it feel great and nerdy &#128520; ?
Now you are ready to explore the possibilities of Termux. Get out and explore. 

### A word of caution - &#128565; Do not clone and run anything you come across. 
Not all the code you see will be safe . There may be malicious code as well. Inspect the code once before you execute something. If you are not very sure , do some googling about that repo. If you sespect something do not execute. 

Stay safe and enjoy. &#129321;

