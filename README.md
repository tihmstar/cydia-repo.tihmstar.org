cydia-repo.tihmstar.org
==========

This repo is not meant to be clone by regular user.
If you want to get it's content you should add "repo.tihmstar.org"
and download the tool via Cydia or apt.

This is a cydia undeb-repo.
If you want to maintain your package hosted on my repo, 
you need to (ask me of course first and then) make such a undeb-repo on your git. 
There you can push your changes and my daemon will clone your git repo, 
build a deb and push to my Cydia repo.


You need to create a new repo in your git which must be named "cydia-repo.tihmstar.org"
In the README.md i advise you to copy the first part from this file.
Here you create a dir for each package you want to sumbit and name it with the package ID. (here i have org.tihmstar.part-fuzzycactus)
Inside this package dir you put basically everything in what you would put in a deb.
All files will be extracted to / when you install that package on the iDevice.
Also you must have a header a "DEBIAN" folder.
Inside that you must have a "control" file which must contain 
"Package" (id of your package)
"Name" (name displayed in cydia)
"Version" (your package version)
"Author" (your name)
feel free to look at the control file inside this repo ;)
