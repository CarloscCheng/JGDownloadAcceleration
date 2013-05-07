<h1>JGDownloadAcceleration<h1> <h5>© Jonas Gessner 2013</h5>

------------------

JGDownloadAcceleration is a Networking library for iOS targeted at downloading large files on to the device's hard disk.

JGDownloadAcceleration's main part is a concurrent NSOperation subclass (JGDownloadOperation) which handles the multipart download.

For managing and queing multiple operations, JGDownloadAcceleration provides a NSOoperationQueue subclass (JGDownloadOperationQueue) which handles the networking thread, activity indicator and application background task.


Q. How does the download acceleration even work?

A. Download accelerators (multipart download) use multiple network connections to download a file from a server in chunks (each connection downloads one part of the entire content). This allows to bypass bandwidth limitations set by the server and download speeds can be drastically increased.

More info: <a href="http://en.wikipedia.org/wiki/Download_manager#Download_acceleration">Wikipedia</a>


The server from which downloading a content needs to support the `Range` header in order to use multipart download. See <a href="#requirements">Requirements</a> for more Info.

##Getting started

1. Download JGDownloadAcceleration
2. Add the whole JGDownloadAcceleration folder to your Project

##Overview
##Example
##Requirements
##Credits
JGDownloadAcceleration was created by <a href="http://twitter.com/JonasGessner" target="_blank">Jonas Gessner</a>.
It was created for the iOS Jailbreak tweak "ProTube Extension for YouTube" and the Jailbreak App "ProTube".

##License

JGDownloadOperation is available under the <a href="http://opensource.org/licenses/Python-2.0">Python 2.0 license</a>
