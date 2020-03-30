# EXP02: Exploratory Project 02
Due on Monday April 20, no later than 5:00 PM

## Overview

In this project you will work with code from an open source project.  Remember that the project is a vehicle to allow you and your teammates to demonstrate your facility with a methodical process for both dealing with bugs and adding new features, as well as the tools to support building high quality software.

## NOTE
The project includes some image files.  Two of the image files were apparently too large for the GitHub classroom service (though GitHub itself was fine with them).  You can grab the two large image files from [this shared Google Drive folder](https://drive.google.com/open?id=1t5WSMtZvior5Fn2qIaDVr5TcV976dqcA), along with a text file with source and licensing information.  You *should* be able to add them to your cloned copy of the repository.  The image files are zipped, so you will need to unzip them before you can use them as tests inputs.

You do NOT need to push those large image files back to your GitHub repo.


## Advice

Use git, branches, frequent commits, and commit comments to document what your process is.  For example, when tracking down a bug you are expected to create a bugfix branch (and document the bug you're fixing in the commit comment), write tests that reveal the bug on that branch, implement a fix on that branch, and once the tests pass, merge back into the main branch.


## Scenario

You are working for [Q](http://jamesbond.wikia.com/wiki/Q) at [Universal Exports](http://jamesbond.wikia.com/wiki/Universal_Exports).  You and your crack cyberteam have to find a way for [007](http://jamesbond.wikia.com/wiki/007) to communicate surreptitously communicate with [M](http://jamesbond.wikia.com/wiki/M).

You come across the idea of [steganography](https://en.wikipedia.org/wiki/Steganography), and have found [an implementation on-line](https://github.com/hiteshd/Steganography-by-LSB).  **_Although the code is available via the project's git repo, use the source provided to you in this repo, in case any updates are pushed to the live repository._**

Bond has uncovered a nefarious [Spectre](http://jamesbond.wikia.com/wiki/SPECTRE) plot, and needs to send both some text and a photo.  But, heavens above, Spectre sabotaged the code!


## Tasks

### MAKEFILE
Add a makefile to support proper unit testing, coverage checking, and making the code to support any other tool you need to use.


### BUG 1
Look at the imgX.bmp and corresponding imgX_steg.bmp files in the images directory.  The '_steg' files encode a message.  They should be visually indistinguishable.  However, they are not.

Try to fix the problem.


### FEATURE REQUEST 1
The code only allows text to be hidden within an image.  Modify
the code to permit another image to be hidden.  Spell out the
size, color depth, or other restrictions on the image to be
hidden, relative to the image in which is it hidden.

Add command-line arguments "-text" or "-image" to specify whether
text or image data is to be hidden, respectively.

Try to add this feature.


### FEATURE REQUEST 2
    
The code only works with images in the .bmp format.  Extend it to
work also with files of different image formats, such as .jpg,
.tiff, .raw and .gif.

Have the program deduce the file type automatically from the
extension on the filename.  If an unsupported file type is used
with the program it must exit with an appropriate message.

You may use other existing libraries to help implement this
functionality (e.g. a library to convert between formats) as long
as
1. the library's licensing permits it (add the library's license as a text file to your repo), and 
2. you give proper credit.

Try to add this feature.
