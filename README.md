# XboxDevModeBatchScripts
A collection of useful batch scripts created by me and community members during my security research of the Xbox One/Series, specifically for Dev Mode SystemOS.

### SystemTelnet
Provided the executing shell has Admin privileges, this script will abuse XRun to run telnetd as SYSTEM on port 23. Credits to Team XOSFT.

### DumpSystemOS
This script fairly automates the process of self-dumping SystemOS via way of xcopy. A directory named the current SystemOS version (Parsed from VER) is created on D:\DevelopmentFiles, followed by nested folders for each drive. The script then executes xcopy with a range of parameters to copy as many files from what I consider "essential drives" for reverse engineering and other research to their respective folders, leaving all for the user having to do is copy the dump folder to their PC.

### RemoveTelemetry 
Provided the executing shell has SYSTEM privileges, this script will disable the known Xbox telemetry services for this boot. Note that this script must be ran every reboot as the services being disabled and deleted is not permanent due to the (mostly) read-only registry. 
