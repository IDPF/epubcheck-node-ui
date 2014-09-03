EpubCheck Node UI
=================

The node server provides a simple UI that wraps epubcheck.  

## Setup
To setup the server:
```
$ npm install.
```

## Running
To run the server type 
```
$ node checkserver.js
```
If you use the '-h' option you will see the various options that are available.
Once the server is running, browse to http://localhost:port#.  The default port number is 8080.

The 'Check Messages' tab is for modifying the overrides files used by epubcheck.  By default it lists all messages that epubcheck can emit.

The 'Comparison' Tab is for comparing the output between two versions of the same epub.

All of the other tabs provide information about the epub selected in the 'Files' tab.

## EpubCheck Version
If you need to update the version of epubcheck that the server is using run:
```
ant clean setup -Depubcheck.version=nnnnn
```
This will compy the necessary dependencies into the epubcheck folder.  After the update has been made the changes will need to be checked in.
