# Install Mozilla Binaries Script

**By:** Ryan Chapin [Contact Info](http://www.ryanchapin.com/contact.html)

Automates the download, verification and installation of distributions of mozilla binaries.  Currently, supports firefox and thunderbird and any other binaries that follow the same directory layout on the ftp.mozilla.org download site.

Initially written as I was running CentOS 6.x on a desktop machine and wanted to make sure that I had the latest and greatest of both Firefox and Thunderbird.  As CentOS did not continually update the RPMs with the continuous changes made to those two code bases I was tired of having to manually download, check the hashes of the downloaded files and 'install' them on my machine.

Since, I have expanded the script to run under Win and Mac with a bash interpreter.  For those operating systems, if the user so desires, they can use this script to automate the download and checking of the hashes of the latest version of Firefox and/or Thunderbird.

Please see the script and the config file themselves for complete documentation.

## To Install

- Download the ```install-mozilla-app``` script and make sure that it is executable.
- Download the ```install-mozilla-app.conf``` configuration file and place it in /etc
   - If you are running under Windows edit ```install-mozilla-app``` and search for ```# Pull in the user configurations``` and update the path to wherever it is that you decide to put the .conf file.
- Edit ```install-mozilla-app.conf``` and configure for your OS, language, and the installation and temp directories that are specified.  Make sure that those directories are writable by whatever user is going to run the script.

