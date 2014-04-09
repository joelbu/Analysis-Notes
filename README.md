Analysis I/II Notes
===================
This repo contains all the handwritten notes from Professor Imamoglu's Analysis I/II class for CS at ETHZ. 

<a name="Getting the material"></a>
Getting the material
====================

In order to get the material, there are two ways:

* Get a .zip file, containing all of the notes. This version might not be as up to date as the source files, but it is usually corrected and checked. Use this option of you are not familiar with LaTex or GitHub
  1. Download the .zip archive [here](https://github.com/pennatil/Analysis-Notes/archive/master.zip)
  2. Unzip it, you will find a folder named "Notes", open it
  3. Find a folder named "Output"
  4. Get the files you need
* Typeset (Build) it yourself from source. This is in order to have the latest version available (like bleeding edge)**(WARNING: MIGHT CONTAIN ERRORS IN THE TEXT)**. Take a look at the [Building](#Building) section

<a name="Contributing"></a>
Contributing
============

Since these documents are still a very early version, they might contain a few (if not more) mistakes. Also, not everything has been yet typed up. You can help in two ways: 

1. Correct mistakes you find in the notes
    * If you have no experience with LaTex or GitHub:
    	1. Make sure you have a GitHub account, otherwise create one [here](https://github.com/join). Please use the same name as your ETHZ account, makes my life much easier if I have to contact you.
		2. On the right side of this page, click on the "Issues" tab
		3. Check if no one else has posted the same Issue. If no one has, open a new issue, stating:
	 		 * Chapter + Page Number
	 		 * Issue found, plus the eventual correction(s)
	 		 * Tag: Add a tag that best classifies the issue
		4. Post the issue, it will be corrected ASAP.
	* If you are familiar with Latex and GitHub:
		1. Fork the repo. Help [here](https://help.github.com/articles/fork-a-repo)
		2. Make the changes, and commit them to your forked repo. Make sure to add detailed comments explaining what you changed, makes my life a lot easier when merging!
		3. Once you are done, request a Merge. Help [here](https://help.github.com/articles/using-pull-requests)
2. Type up what's left of the notes
	* Only for people familiar with LaTex and GitHub. In this case, <a href="mailto:pennatil@student.ethz.ch?subject=I%20want%20to%20help!">contact me</a>.

I will not take into consideration emails containing corrections. Please use the "Issues" tab so to keep track of every change.

<a name="Building"></a>
Building
========
This is only recommended to people with experience with LaTex, since the files might still contain bugs and errors that have to be ironed out. I will not answer emails asking for help if the files do not build! If you are not sure, just use the PDFs inside the .zip archive (Take a look at [Getting the material](#Getting the material)).

1. Make sure you have a working Tex distribution installed on your system. If you don't:
	* Mac OS: [MacteX](http://tug.org/mactex/)
    * Windows: [MikTeX](http://miktex.org/download) or [TexLive](https://www.tug.org/texlive/acquire-netinstall.html) (Recommended)
    * Linux: [TexLive](https://www.tug.org/texlive/quickinstall.html) (or simply <code>sudo apt-get install texlive-full</code>)
2. Download the master Branch [here](https://github.com/pennatil/Analysis-Notes/archive/master.zip)
	* If you want to use a program with a GUI:
	  1. Navigate to the "MAINs" folder, and open "main.tex" using TexWorks (Right-click->open with...)
	  2. On the top left, select "pdfLaTex" from the dropdown menu
	  3. Click on the green arrow, this will start the building process. Repeat this step at least 2 times!!
	  4. Navigate to the Notes folder, you will find a PDF file named "main.pdf". Move it and rename it wherever you like.
    * If you want to use the terminal (Linux and Mac only):
	    1. <code>cd path/to/MAINs/folder/</code> (e.g. <code>cd /Users/Waldo/Desktop/Notes/MAINs/</code>)
   	    2. There are 2 scripts that take care of building the files, and cleaning up. <code>BuildAll.sh</code> builds 1 pdf with all the notes, while <code>BuildChapterByChapter.sh</code> builds a file for each chapter. choose which one you want to use, and follow the commands.
		3. If it is the first time that you run this script, type <code>sudo chmod 755 nameOfScript.sh</code> (Where nameOfScript.sh is either BuildAll.sh or BuildChapterByChapter.sh. This command grants permission to the script to run)
		4. Afterwards, <code>./nameOfScript.sh</code>
		5. You will find a folder called "Output" inside the Notes folder, with the output file(s).

