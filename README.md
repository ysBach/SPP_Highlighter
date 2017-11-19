# SPP Highlighter

This is a highlighter for SPP language, a language used for IRAF ([Official](http://iraf.noao.edu/), [Wikipedia](https://en.wikipedia.org/wiki/IRAF)). 

Basic structure of the syntax file is heavily based on the C sublime-syntax from [``Sublime Text``](https://github.com/sublimehq/Packages). 

**It is partly a result of my own research and the TA material of the *Astronomical Observation and Lab 1 and 2* courses offered at Seoul National University, in 2017.**

What the heck is SPP? From STSDAS web archive:

> Most IRAF and STSDAS applications are written in **SPP**, or Subset PreProcessor, which is *the native programming language of the IRAF system*. SPP is based on RATFOR--rational Fortran--and combines the familiarity of Fortran with some features of the C programming language.



First, how to download and install, and then the philosophy of making this highlighter:



## Download & Installation

Download this repo by either

1. clicking ``Clone or download`` button on the top right and clicking ``Download ZIP``, and unzip it,
2. typing ``git clone https://github.com/ysBach/mdnotes.git `` on the terminal. You may need [Git](https://git-scm.com/downloads) for this.

Then move the (unzipped) directory (or folder) to an appropriate place. 

-----

For example, for [Sublime Text 3](https://www.sublimetext.com/3):

* Windows: ``%APPDATA%\Sublime Text 3\Packages\User``
* OS X: ``~/Library/Application Support/Sublime Text 3/Packages/User``
* LINUX: ``~/.config/sublime-text-3/Packages/User``

Other editors, e.g., [MS Visual Studio Code](https://code.visualstudio.com/docs/extensionAPI/language-support), there should be appropriate ways like writing a json file.

-----



## Purpose

First of all, I am not a programmer, developer, or a computer scientist. Neither am I practiced so. I got to know some terms like ``tmlanguage`` or ``sublime-syntax`` file only ~ 1 day ago. But due to some reasons, I had to make some small effort to this work (the main structure of the syntax file is from Sublime Text, see ``LICENSE.md``). This is never intended to be regarded as a perfect work, and I may not be able to maintain or update this repo.

### Reasons

Although it's been decades since SPP appeared and number of astronomers use IRAF, **there is no single highlighter for SPP or CL script I could find**. While preparing for the TA material, I had to crosscheck my python code with IRAF. Then I found IRAF is not always giving results as expected. This includes centroiding and aperture photometry.

Alongside with some problems in IRAF, I needed to check the internal codes of IRAF for the preparation of my TA material, since I couldn't find ANY detailed manual of IRAF which explains the detailed algorithm implemented to tasks of IRAF. I am sure there are extremely few people who know how the aperture trace, cosmic ray rejection, photometry, or centroiding is working in IRAF. This is critical since it means only those people can understand the results. While looking inside IRAF, the highlighter was quite necessary.

First, I didn't care much about jargons like ``keywords`` and ``conditionals``, but then I changed my mind to copy and modify the pre-existing syntax file. This is the result of such modification to the pre-existing syntax file. I have never, and will never study SPP heavily, so the syntax file may contain many wrong classifications, but anyway the "coloring" itself works correctly, and it fulfills my original purpose. So I stopped modifying it further and made this repo.









