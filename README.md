
![CC Graphics 2024_TextEditor](https://github.com/csae-coders-corner/An-alternative-text-editor-to-write-and-run-your-Stata-code/assets/148211163/33287e83-1d24-4295-af27-36a2f56d6e09)

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

![texteditor2](https://github.com/csae-coders-corner/An-alternative-text-editor-to-write-and-run-your-Stata-code/assets/148211163/2d9de994-d8d4-4a25-99e7-511578e2d740)

  - Now search for “StataEditor” and just click on it to install:

    ![texteditor3](https://github.com/csae-coders-corner/An-alternative-text-editor-to-write-and-run-your-Stata-code/assets/148211163/52144c0a-b856-40c6-b405-8ed41e017ec5)

  - **Install Pywin32**: repeat steps “a” and “b” above, but now installing the “Pywin32” package.

  - **Configure StataEditor**: In ST3 go to the top menu and click on Preferences > Package Settings > StataEditor > Settings - User. In the file that will open, you will have to write the path to your Stata executable (make sure you check if your Stata is SE? or MP?) and the version. For example, my configuration file in Windows looks like this:

![texteditor4](https://github.com/csae-coders-corner/An-alternative-text-editor-to-write-and-run-your-Stata-code/assets/148211163/2fba2df7-b282-4806-a12b-90d9f0b76501)

  - **Register Stata Automation library**: go to the Stata executable (.exe) for which you copied the path (e.g. StataSE-64.exe) and create a shortcut for it (on your desktop). Now right click on this new shortcut and select “Properties”. In the “Target” field, add “ /Register” at the end (with a preceding space).” As in:
"C:\Program Files\Stata16\StataSE-64.exe"  /Register

![texteditor5](https://github.com/csae-coders-corner/An-alternative-text-editor-to-write-and-run-your-Stata-code/assets/148211163/f965ebd2-1175-42fc-bfb7-cbf40ee58bb7)

  - Apply and accept the changes and right click again on the shortcut and choose to “Run as administrator”. Job done, nothing will happen, but if all the steps run smoothly, you should be ready to start using ST3 to write and run Stata code.

  - Just to confirm, restart ST3 and open an existing do-file (or create a new one saving it with a .do extension). You should read “Stata” on the bottom right corner, and should be able to execute selections or complete do-files with Ctrl+D.

**Another useful [reference for Sublime Text commands is available here](https://sublime-text-unofficial-documentation.readthedocs.io/en/latest/reference/commands.html).**

**Giulio Schinaia, DPhil Candidate in Economics, Balliol College, and Research Assistant at the Mind and Behaviour Research Group, Blavatnik School of Government, Oxford, 20 January 2020**
