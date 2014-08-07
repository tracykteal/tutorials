# mothur tutorial


### Logistics
Instructor:
Tracy Teal <tkteal@msu.edu> @tracykteal

Real-time notes for the class.  These will stay there after the workshop too.
<br>Etherpad:  http://epad.hpcc.msu.edu/p/mothur_Illumina_workshop

shell cheat sheets:<br>
* http://fosswire.com/post/2007/08/unixlinux-command-cheat-sheet/
* https://github.com/swcarpentry/boot-camps/blob/master/shell/shell_cheatsheet.md

### Overview of mothur
What you can use it for and what is the workflow

#### Running mothur
You can run mothur on your own computer.  To do this, you would just download mothur

http://www.mothur.org/wiki/Download_mothur
<br>(we're not going to talk about the GUI version)
But you can also run mothur on a server, Amazon or an HPCC.  The advantage of this is that it's not taking up computational resources on your own computer.  You could even start something and then close your computer and go home, or I mean come back in to work.  

The files that you need are in the shared space. We're going to access the files from there,
but do the analysis in our home directories.

Let's get ready to run mothur.  This server uses the module system, so we just type  
`module load mothur`

And then type  
`mothur`  
Now you're in mothur, and we can start!  
And the first thing we'll do is quit mothur, so type  
`quit()`  

Go to the mothur MiSeq SOP
http://www.mothur.org/wiki/MiSeq_SOP

We already have the files we need for this example, but let's take a look at some of them.  To see what files you have type  
`ls`  
Now you see a list of files.
We have the fastq files.  Those are the files you get back from the sequencing center.
Then you have the stability.files file.  That is a file that tells mothur what paired end sequences go together and what the sample name is.  Let's take a look at that file.


You can see that the format is a tab delimited file with the sample name in the first column,
the forward read in the second column and the paired end read in the third column.  
You could create this file in Excel, then save it as a tab-delimited file.
It doesn't have to be called stability.file.  You can call it whatever you want.  The 'stability' part is just what it's named in the example.

Now let's start mothur again.  Type  
`mothur`  
And we're back in mothur, and let's start going through the protocol

** Often the summary.seqs() commands take awhile.  Just wait and eventually you'll get the result


### mothur example
