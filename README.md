Orthanc On Windows 
===================

This project contains the following windows specific extensions for Orthanc:

* OrthancSerivce - A C# Windows Service that will launch the Orthanc server (and restart it if it crashes)
* OrthancInstaller - A NSIS installer for Orthanc. 
* ConfigurationFileWriter - A C# console application that will patch the configuration files during installation based on the selected folders

Building
========

Pre-requisites
--------------

1. Visual Studio 2013 Professional (may work on other versions but has not been tested)
2. NSIS 2.46 (may work with other versions but has not been tested)

Building The Installer
----------------------

1. Open the solution, make sure "Release" is your active build configuration 
2. Copy the build of Orthanc.exe you want to build into the installer into the "InstallerAssets" directory.  Note that the exe must be named Orthanc.exe!
3. Build the solution (F6)

If everything builds OK, the installer will be located in OrthancInstaller/OrthancInstaller.exe

