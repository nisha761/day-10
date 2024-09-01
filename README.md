compramising a machine:A compromised machine refers to a system that has been infiltrated by software pirates, who use it to host download sites for unlicensed software, media files, and other similar items. This compromises the machine's network and storage resources and may result in a denial-of-service attack to other systems or resources on the network.
Volatile Data Collection Steps
•
On the compromised machine, run a trusted command shell from a toolkit with statically compiled binaries (e.g., on older nonproprietary versions of the Helix CD or other distributions).

•
Run script to start a log of your keystrokes.

•
Document the date and time of the computer and compare them with a reliable time source.

•
Acquire contents of physical memory.

•
Gather host name, IP address, and operating system details.

•
Gather system status and environment details.

•
Identify users logged onto the system.

•
Inspect network connections and open ports and associated activity.

•
Examine running processes.

•
Correlate open ports to associated processes and programs.

•
Determine what files and sockets are being accessed.

•
Examine loaded modules and drivers.

•
Examine connected host names.

•
Examine command-line history.

•
Identify mounted shares.

•
Check for unauthorized accounts, groups, shares, and other system resources and configurations.

•
Determine scheduled tasks.

•
Collect clipboard contents.

•
Determine audit configuration.

•
Terminate script to finish logging of your keystrokes by typing exit.

Analysis Tip
File Listing
In some cases it may be beneficial to gather a file listing of each partition during the live response using The Sleuthkit (e.g., /media/cdrom/Linux-IR/fls /dev/hda1 -lr -m / > body.txt). For instance, comparing such a file listing with a forensic duplicate of the same system can reveal that a rootkit is hiding specific directories or files. Furthermore, if a forensic duplicate cannot be acquired, such a file listing can help ascertain when certain files were created, modified, or accessed.

