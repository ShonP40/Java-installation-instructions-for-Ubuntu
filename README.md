# Java installation instructions for Ubuntu
Installation instructions for installing Oracle Java JDK 8 64-Bit on Ubuntu 16.04-20.04

1. Go to [Oracle's website](https://www.oracle.com/java/technologies/javase-jdk8-downloads.html) and download the latest Linux x64 Compressed Archive.
2. Open Terminal and type `sudo mkdir  -p /opt/jdk`.
3. Go to your Downloads folder (or the folder that you downloaded the file to) and open Terminal from it (by right clicking and selecting "Open in Terminal").
4. Type `sudo cp -rf jdk-8u(version number)-linux-x64.tar.gz /opt/jdk/`.
5. Type `cd /opt/jdk/`.
6. Type `sudo tar -zxf jdk-8u(version number)-linux-x64.tar.gz`.
7. Type `sudo update-alternatives --install /usr/bin/java java /opt/jdk/jdk1.8.0_(version number)/bin/java 100`.
8. Type `sudo update-alternatives --config java` (It prompts for selecting by 0,1,2..so choose the version that you downloaded).
9. Type `sudo  nano /etc/environment`and paste `JAVA_HOME=/opt/jdk/jdk1.8.0_(version number)` and `JRE_HOME=/opt/jdk/jdk1.8.0_(version number)/jre`
10. Verify your installation by typing `java -version`.
