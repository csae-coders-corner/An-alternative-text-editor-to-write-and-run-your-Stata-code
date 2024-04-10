# An-alternative-text-editor-to-write-and-run-your-Stata-code
Do you spend a lot of time opening and closing different do-files looking for a particular line of code?

Do you often keep switching across different do-files a lot during your session?

Do you wish you could edit the multiple lines of code at the same time?

If you answered ‘yes’ to any of the questions, you should read on – especially if you have not tried any alternative text-editors other than the in-built do-file editor.

**[Sublime Text](https://www.sublimetext.com/) can change your coding experience using Stata!**

I have found text-editors not as common among the average Stata-user as for coders in other languages. They can be quite timesaving relative to the standard do-file editor Stata offers: they are, basically, an alternative to the do-file editor from which you can write and run your code.

In this post, I will talk about one particular text editor (Sublime Text), but there are many alternative text editors available – so you should shop around.[^1] Sublime Text takes very little installation time (5-15min) and can save you a lot of time during your coding just by using some of its more basic features. There are many more features available, which go beyond the scope of this post.
[^1]:Sublime text can be trialled for free perpetually – users can purchase a $70 licence, which avoids a reminder every 20 saves. Another popular text editor that can be integrated with Stata is Atom, which one you choose seems a matter of personal preference.

**Some basic useful shortcuts and features in Sublime text:**
- **Ctrl+P**: lets you open do-files anywhere on your disk (without the click of your mouse!).
- **Ctrl+Shift+F**: lets you search for a particular string of code across multiple files in a folder.
- **Ctrl+click**: lets you select multiple lines simultaneously to then write code on all of them (no copy-and-paste).
- You can create your own shortcuts using the dropdown menu Preferences/Key Bindings!
- Working from a Sublime “Project” lets you re-open all the do-files you had open from the previous session simultaneously whenever you need.
- **New View into file** (see screenshot below): lets you work simultaneously on two windows of the same do-file (automatically saving any changes to both windows, not just one as in Stata).
- **Automatically fills** previously used macros or variable names as you start writing them.

A screenshot of the Sublime interface:

## How to set up Sublime Text to interact with Stata

1.	[Download and install Sublime Text 3 (ST3) here](https://www.sublimetext.com/) for your operating system.
2.	Open ST3 and install its “Package Control” package following [this 2-step guide](https://packagecontrol.io/installation):
- Open the command palette pressing: ctrl+shift+p (for Windows) or cmd+shift+p (for OS X).
- Type ”Install Package Control”, press enter.

4.	Below I quote a useful [post](https://acarril.github.io/posts/use-st3#stata) by [Alvaro Carill](https://acarril.github.io/), which explains how to install the Sublime packages needed (and simply add a few screenshots):

 - **For OS X**: Install [Stata Improved Editor](https://github.com/zizhongyan/StataImproved) by opening the command palette in ST3 with Cmd+Shift+P, type “install” and hit Enter. Search for “Stata Improved Editor” and just click on it to install. Reboot ST3 and job done!

 - **For Windows**: Install [Stata Editor](https://github.com/mattiasnordin/StataEditor) following these steps:[^2]
[^2]: A step-by-step video of the installation of Sublime Text and its package StataEditor is also here.
 
  - In ST3, start the command palette with Ctrl+Shift+P, type “install” and hit Enter”:




