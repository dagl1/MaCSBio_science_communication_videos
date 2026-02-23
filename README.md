# Description
This repository contains the files necessary for creating animations of MaCSBio-derived algorithms for educational and science communication purposes. It also includes the videos themselves as well as instructions for student projects (MSP and others) on how to contribute to this repository. 
# Table of contents

  - [Examples/highlights](#examples-and-highlights)
    - [[DEMO]: Route optimisation](#route-optimisation-(demo))
    - [3Blue1Brown video](#3blue1brown-video)
  - [Student project description](#student-project-description)
  - [Resources](#resources)
    - [Git tutorials](#git-tutorials)
    - [Git](#git)
      - [Create a Github account](#create-a-github-account)
      - [Installing Git](#installing-git)
      - [Setting it up](#setting-it-up)
      - [How to use Git](#how-to-use-git)
      - [Using Git daily](#using-git-daily)
    - [Manim resources](#manim-resources)
      - [Python and Manim ce](#python-and-manim-ce)
      - [Manim Video](#manim-video)
      - [Sublime](#sublime)
      - [Manim API](#manim-api)
  - [Project instructions](#project-instructions)
    - [Storyboarding](#storyboarding)
    - [Scene and file management](#scene-and-file-management)
    - [Coding tips](#coding-tips)
  - [Report](#report)
    - [Writing tips](#writing-tips)
  - [Presentation](#presentation)
    - [Presentation-tips](#Presentation-tips)
  - [Problems](#problems)
  - [Additional repo information](#required-installations)


## Examples and highlights
  ### Route optimisation (demo)

 https://github.com/user-attachments/assets/07aae5cb-d3b7-4ec1-8373-060e028a7292

  ### 3Blue1Brown video 

  [[!video](https://i.ytimg.com/vi/fNk_zzaMoSs/hqdefault.jpg)](https://www.youtube.com/watch?v=fNk_zzaMoSs&list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)

  The code for this 3Blue1Brown video can be found [here](https://github.com/3b1b/videos/blob/master/_2016/eola/chapter1.py).

________________________________________________
## Student project description
  As the Examples section shows, Manim is very versatile and capable of creating
  intuitive examples. The goal of the stutdent project is to design and produce a video
  that shows off the various methods created at MaCSBio. Initially we start with my
  (Jelle Bonthuis) transcriptomics -> enzyme capacity methods for constraint-based
  metabolic modeling. Subsequently, these enzyme capacities are used in an algorithm
  called SWAMP, which is what the route optimisation demo is about. If time allows I
  hope you can create both as they tie in together. 

  In later projects, we will tackle other methods or algorithms created by colleagues at
  MaCSBio.

________________________________________________
## Resources

### Git tutorials
As I would like you to use git, which is scary (it was for me for a
long time, and I do a lot of computer-related work and programming), especially
in the beginning. Theoretically if you follow the instructions of commiting,
pushing, pulling changes, and no-one modifies other peoples' files, then no problems
should emerge. However you will likely get a "merge conflict" or "commit merge
changes" popup, which you can google or look into. The links below are there to help
you (even if it takes a little bit, putting in the effort to have a basic
understanding of git will likely help you in your future). 

  - [many good links, some included later](https://gist.github.com/jaseemabid/1321592)
  - [a beginner's guide to git commits](https://medium.com/@zacyap/a-beginners-guide-to-git-commits-34185ed2ed8d) 
  - [full git usage guide, this is linking to the saving changes part](https://www.atlassian.com/git/tutorials/saving-changes)
  - [w3schools guide if you prefer their style](https://www.w3schools.com/git/git_commit.asp)
  - [common github errors and solutions](https://medium.com/devops-ai-decoded/common-github-errors-and-solutions-cd464f0db2b5)
  - [often encountered errors](https://graphite.com/guides/debugging-common-git-errors)
  - [git cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf)
  - [visual guide](https://marklodato.github.io/visual-git-guide/index-en.html)     
  - [simpler git](https://nfarina.com/post/9868516270/git-is-simpler) 
  - [git for the lazy](https://wiki.spheredev.org/index.php/Git_for_the_lazy)
  

### Git 
As you are working together on code that will be hosted on github (here), using Git is
essential. If you are not familiar with Git, 
it is the most-used type of version control (the ability to see previous versions, and
to "go back" to them without necessarily losing other progress). Especially in
programming/software projects where multiple people work together and might all edit
similar code/files, this became crucial. See this (somewhat not-serious video) that
explains how useful this was: 

[![Video](https://i3.ytimg.com/vi/iaEnUXtiGsE/maxresdefault.jpg)](https://www.youtube.com/watch?v=iaEnUXtiGsE)

### Create a Github account 

- Follow the instructions [here](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github)
(I recommend using your personal email, as your university email will eventually 
become inaccessible).
- Become collaborator to this Github by sending me the name of your account name, so I
  can send you an invite which you will have to accept on Github (you will see an
  message popup and get an email on the adress you registered).

### Installing Git

If you are a Linux user, I assume you can follow the instructions [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git). 

#### Windows

Installing Git on Windows is straightforward: 
 - Download the latest version of *git for Windows* [here](https://gitforwindows.org)
 - Follow the installer instructions, and if given the option, choose to use Git Bash instead of the standard Git Windows Command Prompt.
 - After installation is complete, verify that it is working by opening Git Bash and typing `git --version`; you should see `git version 2.45.1.windows.1` or something similar.

 (Optionally) If you rather use a GUI instead of having to use the command line, you can
 install Github Desktop - *in addition to Git, **not** as a substitute*; do note that
 while this is easier 95% of the time you might run into an issue and will require Git 
 Bash, and learning the few Git commands you need won't hurt you (and is valuable 
 in many settings).
 - https://desktop.github.com/download/
 - Follow the setup instructions
 - Login to your Github 

#### Mac 
Similar to installing on Windows, installing Git on Mac is fairly straightforward. The
instructions can be found [!here](https://git-scm.com/install/mac) and are as follows
(using brew, the link has several other options including MacPorts and Xcode):
- install homebrew by pasting this into the macOS terminal: ```/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"```
- type ```brew install git```

 (Optionally) If you rather use a GUI instead of having to use the command line, you can
 install Github Desktop - *in addition to Git, **not** as a substitute*; do note that
 while this is easier 95% of the time you might run into an issue and will require Git 
 Bash, and learning the few Git commands you need won't hurt you (and is valuable 
 in many settings).
 - https://desktop.github.com/download/
 - Follow the setup instructions
 - Login to your Github 


### Setting it up

Once you have it all installed, it is time open up Git bash where we will setup your github account:
Set up an email adress for your github account if you haven't yet, follow these [instructions](https://docs.github.com/en/account-and-profile/how-tos/email-preferences/setting-your-commit-email-address) 

```bash
git config --global user.name "your account name"
git config --global user.email "your email"
git config --global credential.helper manager
```

Then we cd ("change directory") to a git folder, I recommend creating it in a convenient location such as the C drive on Windows:

```bash
cd c:
mkdir github
cd github
git clone https://github.com/dagl1/MaCSBio_science_communication_videos
cd MaCSBio_science_communication_videos
git pull
```
Note that you will probably be asked to login in to your Github account at some point during this process, it will refer you to your browser where you login to your github account.

All other times when you open up git bash, you just need to move to the repository folder. If you are in the c:/git/ folder, and you type MSP then press the "tab" key on your keyboard (above capslock typically), it should autocomplete to MaCSBio_science_communication_videos and you press enter.

### How to use Git

The way of using Git (regarldless of whether you are using Github Desktop, or Git from
command-line interfaces) is to "fetch" (find new changes), "pull" (copy those changes to
your own device), and then after you make changes, you "push" (add changes the central
directory). In this manner, everyone has a central repository, but can make changes
independently. When you and someone else make changes to the same file, you will be asked
to make a concious decision on how to "merge" those changes. In addition there will be a
complete history of all changes you all make to each file. 

### Using git daily

 - Navigate to your repository folder
 - Commit any changes if you made them since your last push:
 ```bash
 git add .
 git commit -m "some message indicating what you added, these can be read back so put in the effort to write what you actually changed"
 ```
The "." in git add . means: add all files on this system
Then, commit is like saying: yes these changes are what we are going to add, write a summary of the changes involved, and get ready to send them to the server (the online Github page in this case). 
  - Alternatively, if you have changes but do not care about them (and want to just get latest version of the server), you can type git stash, which will store/stash your changes (they won't be deleted, but in most cases you won't look back to them).
- You can only push (send to the sever) changes when you have the latest version of the online repository, so you must "pull" that latest version.
- We can only pull if we don't have any open changes floating around, hence we first performed git add/commit or git stash, so that any changes we made are now already set in stone (or stored somewhere else in case you typed git stash). Now that we don't have any open changes, we can type ```bash git pull```. If you didn't make changes to a file someone else made changes too, then it will work wonderfully.
  - It could also show you a different window where it asks you to commit merge changes. Just type something at the top (without #) and then press q, or ctrl+q, or shift+q.
  - If you have changes to file X, but the online version also has changes to file X which are incompatible with yours, it will ask you to deal with this. If this happens, I would look-up or ask chatGPT on how to solve this. Generally it is quite simple in that you need to open the conflicting file, and find places with HEAD and many >>>>>>>>>>>>>>>. These places will show both versions of the file, and you remove one or the other, until no more >>>>>>>>> exist. Then you git commit these changes and the merge will work. This process is somehwat annoying and the first few times scared the hell out of me (and it took me a while to figure out). Don't panic, try to figture it out, ask others, or ask me. And since we are only working with small text files either way, it won't be too much of an issue if you just send the necessary files to other people directly - while you are resolving the issue, don't just stop using git after this happens!
  - After you make changes, such as editing files and adding documentation, you need to go through the git add, git commit, git pull, git push process everytime. To see what changes exist you can type git diff (to see which files are changed, and which are ready to be committed).
 
I know git is scary, but give it a real shot, and otherwise we can go through how to use it too. Even if after this project you aren't going to do anything directly programming related, you will likely come in contact with it at some point in your career.

________________________________________________
### Manim resources

  - [tutorials website](https://docs.manim.community/en/stable/tutorials/index.html)
  - [1 hour long beginner tutorial](https://www.youtube.com/watch?v=KHGoFDB-raE)
  - An "experience" [video](https://youtu.be/5anTYHWuMSA) by a popular youtuber (Bog)
  - A [tutorial](https://www.youtube.com/watch?v=Uy7ceou-iVs) by the same youtuber
    (Bog)
  - A **very** good video of the Manim creator going through the process of making a
    video together with someone who knows nothing about Manim: [link](https://youtu.be/rbu7Zu5X1zI)
  - In the last video 3b1b also goes over his sublime commands, these are useful for
    running and editing, they can be found [here](https://github.com/3b1b/videos/tree/master/sublime_custom_commands)

### Python and Manim ce 
You should install Python, and a version of Manim. If you check the resources you
should swiftly find out that there are different versions of [Manim](https://docs.manim.community/en/stable/faq/installation.html). I personally would go with the most well-documented version: the community edition (ce).
Do note that the demo_route_optimisation was written for the the manimgl version,
however this shoud not matter for your own project (as long as you all use the community
edition).
go with Python 3.14, so all of you will have the same version running. Then follow the
instructions [here](https://docs.manim.community/en/stable/installation/uv.html).
Don't forget to install LaTeX as that will be (potentially) useful for showing the
formulas on-screen.
This repository already contains a pyproject.toml 
file which means you do not have to use the ```uv init``` command. Instead you change
directory (cd) to the git folder; and with uv installed you type ```uv sync``` which
should then show:
``` bash
c:\Git\MaCSBio_science_communication_videos>uv sync
Using CPython 3.14.0 interpreter at: C:\Python314\python.exe
Creating virtual environment at: .venv
```

If you do not have python installed, you might have to install it first using:
```uv python install 3.14```

If you need to add any packages, just run ```uv add PackageName```.

### Manim video 
Also noted in the [resources](#Resources) section, a very good video of 3b1b using Manim
while teaching it to another person ![exists](https://youtu.be/rbu7Zu5X1zI). This is
extremely useful for your overall understanding. Of course you might want to look
into other resources as well, however I personally thought this was very insightful
in how to go about it. Do note he also discusses his Sublime bindings, which I think
are a must-have, as it makes the overall workflow a lot easier.
    
### Sublime
[Sublime](https://www.sublimetext.com/download) is a text editor that can also be used
to run scripts, such as those written in Python. It isn't as versatile as a full IDE
such as Pycharm or Visual Studio, however this is generally not as necessary for small
projects or scripts. Additionally the bindings created for Sublime by 3b1B make it an
ideal choice for this project. Of course you can use whatever you find comfortable to
work with.

### Manim API 
The community edition of Manim has great documentation which can be found [here](https://docs.manim.community/en/stable/reference.html). You of course might need to create your own functions (see the demo_route_optimisation) for an example, the Table that has several cells move and fade, followed by the table it self resizing 
is a custom function, as not everything works exactly as I wanted it out of the box.

I added an example of a custom config in the data folder, which has some options for
eventually creating the video. The Manim instructions will have more information, but at
least with this example you can see what was necessary for me to create the demo video.

________________________________________________
## Project instructions
As we will start with my method called GPRimproved, which integrates gene expression and
converts it to enzyme reaction capacities, we will have a meeting where I will present
this method, and share with you *personally* the method section of the relevant
manuscript. It is very important that you ask a lot of questions and make notes, so that
you can create an accurate video of the method. The aim of the actual video is to
present it to collaborators, and once GPRimproved is published, host it on Youtube for
people to refer to it. It should thus be quite comprehensive, easy to undertand, but not
too long.

### Storyboarding
I recommend you start out by storyboarding, which is the process of creating a "draft"
video, with different scenes and information that you will later create. This will help
both with verifying the accuracy of the information (as the method can be a bit much to
understand immediately), and with finding an intuitive approach for explaining it. It
will be a lot easier to make changes here, than later, and with scenes separated you can
divide the workload among yourselves. 

### Scene and file management
I would recommend working closely together, even
when working on separate scenes, as this will improve coherence and ensure you all use
the same style (agree on a font, overall way of moving things (e.g. fade outs), speed,
and relevant things). 

As you will all be programming, having separate files for each scene is convenient,
especially when having to pull/merge with Git. Additionally, I would recommend creating
utility files with functions that everyone uses, or the settings mentioned such as
speed and font.

Remember that software development is a lot of working together, and so you might have
one person working on a specific animation, while other people use that same animation
somewhere in their scenes. Make the attempt to create functions that can be used by
several people (with arguments for whatever they want to change). Having code repetition
is generally unavoidable though, so don't stress too much about making the perfect
functions or code.

### Coding tips 
Try to typehint your functions, and use comprehensive variable/function names. Don't
write things like "tw = 5 # table width", instead just write out variable names such
that you only need comments to explain the overall idea of your code (and you might not
need any). 
Use a single style: 
  - type hint, using the "typing" library where necessary
  - variable/attribute names are lower_case_and_underscored
  - class names are CapitilizedAndWithoutSpaces
  - class instances are variables and thus lower_case_and_underscored
  - function names are descriptive: create_fade_out_table()
  - lines should not exceed 94 characters
  - follow other [best practices](https://dev.to/devasservice/python-best-practices-writing-clean-efficient-and-maintainable-code-34bj), although don't go overboard; no need for unit-tests, or extensive 
  docstrings. Mostly aim at creating easily readable code that uses the same
  nomenclature and overall structure.

________________________________________________
## Report

### Writing-tips
Academic writing, writing well, and writing very well is a difficult skill to learn.
Writing nice prose is something that is difficult, and which should necessarily be your
aim. Instead your aim should be - in order - be specific, be clear, be concise, write
in a nice manner. 

To be specific means to read what you write and **try** to misinterpret it. Things that
happen commonly is the referring to a particular concept, while meaning something
slightly different. It very often is clear what you *mean*, but what you wrote is not
what you meant. Another common problem in being specific, is the switching of topics
halfway through a paragraph, while not explicitly saying so. 

To be clear, remember to keep the amount of not-explained information to a minimum. When
you discuss a new term, quickly resolve any type of uncertainty. Readers have trouble
keeping many things in memory, so if you are going to discuss a new topic X, don't first
discuss all the ways it can be used, how people think about it, and then explain what
X actually is. It is difficult to properly contextualise the arguments you are
providing, if the reader doesn't yet know what X is. Keep the flow of information
limited and try to organise paragraphs together. Additionally remember to string
together topics in a way where one paragraph feels like it leads into the next. And if
it really doesn't, then adress that. Make sure the reader gets the feeling you are aware
of this abrupt change (you could use a sentence like "Viewed from an entirely different
perspective, one might also ..."). 

For writing concise, write your arguments. Then attempt to reduce unnecessary
information or merge sentences together (this is thus on an information level 
where you might be able to get the same point across, without needing both points);
afterwards you go through it and attempt to reduce the amount of words. Certain ways of
saying things are naturally more wordy than others. Think of: "On the other hand" vs
"Alternatively".

For writing well/nice, tips on the actual wording are difficult. What is important is to
make sure that the reader is taken along in the story, that there is some type of
cadence in the rhytm of your sentences and a paragraphs. Don't have too many super short
paragraphs, don't have too many very long paragraphs. Similarly for sentences,
alternate, try to imagine the reader and how they are feeling (potentially saying the
text out loud in their head) while reading your text. Think of natural pauses, and make
sure that you don't repeat yourself in ways that give the feeling you forgot about the
fact you wrote it before. 

This last point is a common occurence: you might have
discussed topic X in a part, then later you reintroduce the topic as if it is the first
time. Such occurences will feel odd and discordant to your readers. It might indicate
that you didn't reread your story, but moreover it indicates that either before it
wasn't necessary to explain, you didn't believe in your explanation from before (which
then means you wasted the readers time), or you might believe the reader forgot (making
assumptions about your reader). If you do want to harkon back to something, you can
always say: "as discussed earlier, topic X plays an important role in ... the current
results further point to such a role".

I recommend using a citation manager (I personally use Zotero, but any is fine) to add
citations to your document. This is especially nice when you need to use a referencing
style that uses numbers in text: you don't want to have to change the order of all the 
citations because you add or remove single reference. Citations managers will do this 
for you automatically. Similarly, if you need to change referencing style, the manager 
will do so for you automatically. I do realise it might not work that well when writing
a shared document, but as your BTR period follows directly after this, tip might be
useful there even if you can't use it in a shared google docs.


________________________________________________
## Presentation
Obviously the actual animation can be part of the presentation, as it is a very clear
thing you can show. I would organise the presentation around this, by highlighting both
the method itself, how you went about it, why that is important, and then show the
animation. Then you can discuss challenges you came across during the project, and tips
for the future, as well as discussing what could be different or better in the
animation.

### Presentation-tips
A presentation should feel like a concise story, that is well laid out, and that is
presented with confidence. The audience needs to get the feeling that you fully
understand everything about it. Don't make it sound like more or less than you did, be
honest and believe in the value of your work (if you make it sound bigger than it is,
then that implies you feel the value isn't big enough on its own). 

Don't read from slides, don't read from text, preferably don't even have full text
memorised. Try to instead think of a story in your head, think of what the slide needs
to look like for that story, then during the presenation just tell that story. Of cours
you can (and possibly should) rehearse, but rehearsing and memorising aren't the same.
Don't have too much text on your slides, don't make it too fancy, have clear images, and
most importantly, do not repeat your slides except in special circumstances. This last
part happens a lot in student presentations: a slide names several important processes
involved in something, and the student will (without adding anyting) name them all in
order. Sometimes you can't avoid it, but in most cases you could either add extra text,
or mention something like: "it is involved in several processes, which you can see on
screen, the most important ones are x and y".

I personally think that students spend too much time on making presentations look fancy
instead of just neat. I do admit that many people seem to like colours or creativity in
the presentations they observe, however if that takes seven hours, which could have been
spent on improving the logic or flow of the presentation, I personally doubt its
wortwhileness. Neat looking presentations generally have the same information at the
same location (titles always exactly at the same location at the same font size; text
and images generally having designated locations; if using animations, using the same
general order where they appear (if you go left to right once, keep doing that for all
slides)). This helps with keeping people focussed, as they know where to look and
somewhat what to expect. This then also gives you the ability to conciuosly break this
rhytm to make a point or to point something out. Be conscientious with your story
telling!

________________________________________________
## Problems
I very much hope that there will be no problems during the project, neither between your
collaborative effort, nor with my supervision. For the latter, there is always the
possibility to involve my supervisors (the two people also listed for the project), and
of course discuss things with me. 
For interpersonal problems between you (someone not doing anything, a fight, or anything
else), please contact me (preferably after talking between each other) and I can help to
mediate or see if anything is up. Don't wait till the peer-review stage to come with
accusations or comments. Giving and receiving criticism is difficult and uncomfortable
(generally moreso for the receiving part), however it is an important part of working
together, and in many cases one can do so in a civil manner. Neverthelss my office (PHS1
B3.007) is almost always open, and you can always contact me through email or just walk
by! 
Additionally Dr. Daan van Beek will be also part of this project and you can contact him
directly, or come to his office (PHS1 B3.O03).


________________________________________________
FOR MSP PROJECT STUDENTS, NOTE THAT THE REST OF THIS DOCUMENT IS NOT APPLICABLE TO YOU!
**THE FOLLOWING PART IS ONLY REQUIRED FOR SETTING UP SEMANTIC RELEASE AND PRE-COMMIT HOOKS FROM THE BOOTSTRAP REPO.**
________________________________________________
Required installations:

- Node.js (v14 or higher)
  - Download and install from https://nodejs.org/
  - Verify installation by running `node -v` in your terminal.
  - NPM (Node Package Manager) comes bundled with Node.js.
  - Verify installation by running `npm -v` in your terminal.
  - Optional: Install Yarn as an alternative package manager
    - Install via npm: `npm install -g yarn`
    - Verify installation by running `yarn -v` in your terminal.

- Git
  - Download and install from https://git-scm.com/
  - Verify installation by running `git --version` in your terminal.


____________________________________
Required actions:

- Github token setup:
  - Go to your GitHub account settings.
  - Navigate to "Developer settings" > "Personal access tokens".
  - Click on "Generate new token".
  - Select the necessary scopes for your project (read & write access).
    - Contents
    - Issues
    - Pull requests
    - Any additional scopes, eg. workflows
  - Generate the token and copy it securely.
  - Set the token as an environment variable in your terminal:
    - On macOS/Linux: `export GITHUB_TOKEN=your_token_here`
    - On Windows (Command Prompt): `set GITHUB_TOKEN=your_token_here`
    - On Windows (PowerShell): `$env:GITHUB_TOKEN="your_token_here"`


- Clone the repository:
  - Open your terminal.
  - Run the command: `git clone`
  - Navigate into the project directory: `cd your-repo-name`

- Run bootstrap.sh:
  - In the project directory (preferably using git Bash):
`./bootstrap.sh` (macOS/Linux) or `bootstrap.bat` (Windows terminal)
  - This script will install all necessary dependencies and set up the project environment.

________________________________________________

