### Running the Gauntlet ###

The Gauntlet should already be installed on your Rascal. To run it, you execute a script on your Rascal, which connects to another computer on your network that has a special program (Selenium Server) on it. Selenium will use a web browser to test various features by requesting some web pages from your Rascal. Then, it will report back to the Rascal whether it worked.

### Setting up the server ###

This will probably work on Linux and OS X. (Probably not Windows, but whatever. Have fun with your tiles.)

* Download the latest standalone build from http://code.google.com/p/selenium/downloads/list
* Execute: java -jar selenium-server-standalone-<version>.jar

### Starting the test ###

In root directory: git clone git://github.com/rascalmicro/gauntlet.git

pip install sst

sst-remote -d gauntlet -u http://192.168.1.100:4444/wd/hub (but you need the correct server IP address)
