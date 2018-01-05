# linux-info-explorer.sh

Original credit goes to Joe Santoro for the vast collection of resource checks:
http://www.unix-consultants.com/examples/scripts/linux/linux-explorer/

Modifications made to bring it upto date and to include detections for Asterisk/Freepbx configuraitons.


## Usage
login to your PBX. If you are not root you will need to switch to a root user to proceed.

Download the script directly and set it as executable

```
curl https://raw.githubusercontent.com/voice1/linux-info-explorer/master/linux-explorer.sh > /sbin/linux-explorer
chmod +x /sbin/linux-explorer
```

You can not type `linux-explorer` at the command prompt to execute the program.
Follow the onscreen prompts and let the utility run. 

If you have been given specific instructions by support please follow those instructions.

## Submitting the result file.
In many cases your result file may be too big to deliver by email. We recommend uploading the file to dropbox and
sharing a link. 

You should be able to use your file copy tool of choice, WinSCP, Cyberduck, and Filezilla Client are all viable tools.

Once you have file on your desktop you should be able to use any file sharing utility you normally use.
In some rare cases where you do not have access to a file share service, support may ask you to run the utility w/o
collecting LOG data. This may significantly reduce supports ability to provide accurate information however and is not 
advised.

When the script finishes you will see a message like the following:
```
A support file has been created for support purposes


The MD5sum is       : deae36168c83ae798d5d0d7b59adea2f
The Support File is : /opt/LINUXexplo/linux/explorer.007f0100.hostname-2017.01.24.01.32.19.tar.gz

Please send this file and the MD5sum details to your support representative.
```
Please be sure to include the MD5sum and the specified file with your response.




# What is collected?
The script collects different hardware and software configurations. It includes a copy of your /etc directory minus the shadow file.
The script by default will attempt to collect your log files. If you have excessive log files this process may take a long time and result in larger diaganostic files.
The script will attempt to use differnt common tools for information gathering if installed.

