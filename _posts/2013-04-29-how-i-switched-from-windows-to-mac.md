---
layout: post
title: "How I Switched from Windows to MAC"
description: ""
category: Tips
tags: [Migration, MAC, Thunderbird, Firefox]
---
{% include JB/setup %}

I recently got my PC refreshed with a MacBook Air from Company local IT. It was exciting and I felt quite keen to migrate my workspace into MAC. Here I list the steps how I did it for everybody's reference and for my archive purpose. 

If I was given the opportunity of migrating to MAC from Windows earlier like one or two years ago, I would not hesitate a second. But after a long period of exploring, I have collected a category of softwares or applications or tools that are either ease of use or powerful in function and could maximize my productivity and experience, most of which are cross-platform compatible but unfortunately there always is some Windows-only ones that pain you when you lose them.

## 1. Thunderbird

Let me first introduce my work-based email client Thunderbird from Mozilla Corporation. My every job is somehow email driven. I start and end my day by checking and replying email, then work out something and email again during the day. The conventional choice of email client is Outlook of course as most company choose. Also as majorities are complaining, it's slow, complicated, distracting and memory consuming. I don't complain, instead I look to other alternatives. 

I've always loved Firefox so naturally I gave Thunderbird a try. It appealed to me with simple but neat UI, messages sorting, tags, shortcut keys (which is most fascinating), various extensions, and after all that, its fast speed. It took me awhile googling until I was able to connect it with the Exchange server which Outlook uses. Forgive me not to give the details since it's company confidential. 

The effort pays off now as TB is platform-compatible, which means the configurations and emails backups in local machine can be directed copied into MAC and retrieved at once. I'll show you a simple and straight forward way by using _profile_.

### a) Find your profiles
Mozilla applications store your personal settings, added extensions and themes, and user data such as bookmarks, passwords, cookies and mail in a "profile". Everything in one place, cool, isn't it? Let's find it.

	1. Open the Windows Explorer Window.
	2. In the address line, type in %APPDATA%
	3. Under the "Roadming" folder, choose Thunderbird -> Profiles. Each folder in this folder is a profile on your computer.

You can also navigate directly to your profile folder at the following path:
	C:\Users\<Windows user name>\AppData\Roaming\Thunderbird\Profiles\<Profile name>\

### b) Transfer to MAC
Make a copy of the profiles folder and all its sub-folders into destined location in MAC. Be careful not to cut or delete your profiles until everything comes up fine in case you mistakenly lose them forever in the following steps.

Profile folders in MAC OS are by default in one of below locations. You can put your profiles near here with a distinguished name or put anywhere you like and point to it later.
	~/Library/Thunderbird/Profiles/<Profile name>/
	~/Library/Application Support/Thunderbird/Profiles/<Profile name>/
The tilde character (~) refers to the current user's Home folder, so ~/Library is the /Macintosh HD/Users/<\username>/Library folder.

### c) Profile Manager
The Profile Manager allows you create and manage profiles. If you have multiple profiles you can use the Profile Manager to switch profiles. Also
We can make TB to call your own profile instead of default empty one by using Profile Manager.

Close the application completely and make sure that it is not running in the background. Assuming the program is installed in the _Applications_ folder, launch Terminal ("Applications -> Utilities -> Terminal") and enter the command starting with / after the prompt in Terminal:
	/Applications/Thunderbird.app/Contents/MacOS/thunderbird-bin -profilemanager
Adding -bin after the application name is necessary on some systems and application versions. 

Once you've accessed the Profile Manager as described above, click on _Create Profile_ and follow the instructions. Enter a descriptive name for the new profile and and choose the location to where you put your profiles, and then click the Finish button. You can now "Start Thunderbird" and enjoy it.

All of the data is recovered seamless in MAC with same messages rendering, same shortcut keys, no need to worry about formatting or characters showing, that kind of thing. It's quite encouraging.

## 2. Firefox + Pentadactyl

There has been increasing choices of web browsers in the market, top four of which are IE, Firefox, Chrome, and MAC's native Safari. Let alone IE which is most common in non-technical person and least in technical feature, Firefox used to number one. Chrome, however, is overtaking its place year by year for its simplicity and speediness. Safari is good too coming with attractive feature in lately release. 

But I stick to Firefox. And Pentadactyl is the only reason. 

Pentadactyl is an add-on for Firefox, designed to make browsing more efficient and especially more keyboard accessible largely by making it behave like a Vim. 

The migration of Firefox and Pentadactyl is the same as Thunderbird since they come from the same cooperation, allowing some directory name change. 

As to the configuration of Pentadactyl, it worths another article talking about more deeply.

## 3. Gvim

Gvim is my favorite Text Editor, a graphical version of Vim. It is a faith rather than a habit to use Gvim. Fortunately there's MacVim to satisfy you the same. Just copy the _.vimrc_ and _.vim/_ into to your home folder and you're ready to go.

During the Gvim migration I found a great plugin _Vundle_. It creates a _Bundle_ of Vim plugins and categories them into separate folders.

BTW, Sublime Text 2 is awesome too.

## 4. Dictionary

I used Lingoes in Windows. 

The native _Dictionary_ application is the best to me, after adding more dictionary packages. 

## 5. TotalCommander

TotalCommander is a killer resources management tool. Unfortunately there's no alternative in MAC. MuCommander is the most close but still lag a hundred miles away.  




