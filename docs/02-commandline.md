# Commmand Line August 17

If you have time before class, make a short post on something you read about in one of your subscription newsletters. If you have made a forum post, then you may do a starter, if you wish. (You need to first make a forum post before doing a starter.)

If you are having trouble finding the [Technology Review Newsletter signup](https://forms.technologyreview.com/the-download/) Subscription **<<< this link works**.

## Eduroam or VPN

If you do not have access to UNC Eduroam, you must have your VPN client installed and connected before you can log into OPAL.

![vpn image](images/active-vpn-example.png)

## Get to Know the Tilde

It's the <kbd>shift + backtick</kbd> under, or near, the <kbd>esc</kbd> key:

![tilde](images/tilde.png).


## OPAL Accounts Have been Created

!>Important: Replace **<onyen>** with your personal onyen. Example: **opal.ils.unc.edu/~kellyd**

Open a browser and go to:

```
opal.ils.unc.edu/~<onyen>
```  

You should see **Forbidden** message. That is good; that means you have an account, and you need to reset permissions.

Darth Vader **does not** have an account on opal, so he **can't be found**: <https://opal.ils.unc.edu/~darthv>

```
The requested URL /~darthv was not found on this server.
```

My onyen is lblakej. I have an account and I have set my permissions, so you can see my site directory: <https://opal.ils.unc.edu/~lblakej>

```
Index of /~lblakej
```

There is nothing at the opal main page: <https://opal.ils.unc.edu/>; you will just see a blank browser window.

## Learning Objectives

log into OPAL ```ssh onyen@opal.ils.unc.edu```
1. Set up permissions so that I, you, and the world can view your files from a browser
3. create a directory
4. Practice some basic LINUX skills


When you create websites, you should verify your sites with Chrome and/or Firefox. At least use one of these to check/verify your coding. If you are only using Safari, then you are only seeing your site through a Mac "lens." If you are only using Microsoft Explorer or Edge, your are only seeing it as a "PC" user. Also, you need to understand that browsers "cache" pages to save network resources. So it may be necessary to view your website changes in private (Firefox) or incognito (Chrome) mode to see website updates.

## Log in

You can log into your OPAL account with current permission settings. You are going to change permissions to make your public_html directory veiwable to the world wide web.

Here is a permissions calculator to help you grasp the number system [Permissions Calculator](http://permissions-calculator.org/)

How to log in to OPAL
[Link to lecture Command Line web page](https://ils.unc.edu/courses/2020_spring/inls161_001/02a.03.command-line.html)

* Mac Users: Use Terminal
* PC Users: Use Command Prompt or Secure Shell

![password prompt image](images/terminal-password-prompt.png)

## Set Permissions

### Short Version:

```
[your_onyen@opal ~] $
```
Type in: ```chmod 711 .``` **DON'T FORGET THE PERIOD!**

Like this:

```
[your_onyen@opal ~] $ chmod 711 .
```

Press enter. Now you will be able to see your files on the web.

### Longer Version:

Before you (or anyone else) can view your files in a web browser, you must change the access permissions for your home directory on opal. If these permissions are set incorrectly, anyone trying to view your webpage will see a Forbidden error rather than your content. Follow these instructions to set the correct permissions:

Open an SSH connection to Opal.

On Windows, you'll need to use The Command Prompt or Git BASH; on MacOS and Linux, you can open a Terminal window, enter

```
ssh your_onyen@opal.ils.unc.edu
```

and then enter your password when prompted.

Once you've connected, you should see a command prompt like this:

```
[your_onyen@opal ~] $
```

Type

```
chmod 711 .
```

with both the space and the period. If you get a "missing operand" error, make sure you included the space and the period at the end.

## Viewing Your Webpage

After you have uploaded your files and set the correct permissions, your webpage will be viewable at https://opal.ils.unc.edu/~onyen/ . This will take you to the index page in your public_html folder; you can also navigate directly to other pages or subfolders you've added, such as https://opal.ils.unc.edu/~onyen/my_folder/my_page.html

## Create a Directory

<a href="https://ils.unc.edu/courses/2020_spring/inls161_001/02b.02.new-directory.html">Create a Directory</a>

**Grading rubric:** You must follow file naming conventions: **NO SPACES**; no strange characters. Use hyphens or periods where you would have spaces. Try to stick with lowercase letters. After you have created your directory, open the related assignment and paste your link in the submission box.</p>


## Helpful Links

* [Fosswire Unix/Linux Command Reference](https://files.fosswire.com/2007/08/fwunixref.pdf)
* [UNC ITS help sheet](https://github.com/ljonesdesign/161-recitations/blob/master/docs/files/unc-unix-help.pdf)
* [A Command Line Primer for Beginners](https://lifehacker.com/a-command-line-primer-for-beginners-5633909)


## Basics: Command Line Cheat Sheet
[What is the Bash Shell?](https://en.wikipedia.org/wiki/Bash_(Unix_shell))

## Excellent YouTube Command line demos for Mac & PC

*These are optional, but highly recommended if you are interested in pursuing any type of web development.*

* [Absolute Beginner Guide to the Mac OS Terminal](https://www.youtube.com/watch?v=aKRYQsKR46I)
* [Command Line Interface Tutorial (with GitBash)](https://www.youtube.com/watch?v=sw9kdFka8rA) 

If you decide to download [git for windows](https://gitforwindows.org) to tryout GitBash, just install with all of the default items.  

!>The Git GUI will be installed, but you won't need that for this tutorial, and you probably will not ever use it. I don't ever use it. So that could be the one item that you uncheck and don't install.

GitBash is the easiest way to get to play with command line tools like you would on a Mac. Git is another thing altogether, and this video does not get into git or github. It is also possible now to install [Linux Ubuntu as a Subsystem on Windows 10](https://docs.microsoft.com/en-us/windows/wsl/install-win10), but it is too complicated to include in this course.