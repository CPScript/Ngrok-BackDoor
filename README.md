> how to use

* 1. root yourself: `sudo su`
* 2. run script: `python Saturn.py`


# Whats going on??

1. The script first `prints out a banner` and then asks the user to `choose an option`. The options are:
* Linux (Recommended)
* Windows (Harder to use)
* Listen (Connect to a port)
* Exit (Stop this software)
2. If the user chooses the Linux option, the script will ask for an IP address and a port number. It then writes a C program to a file named `.linux.c`. This program creates a socket, connects to the specified IP and port, and then executes a shell `(/bin/sh)`. The compiled executable is saved as Saturn-Linux.
4. If the user chooses the Windows option, the script behaves similarly but writes a C program for Windows instead. The compiled executable is saved as Saturn-Windows.exe.
5. If the user chooses the Listen option, the script `starts a netcat listener` on the specified port.
6. If the user chooses the Exit option, the script exits.
7. After creating the backdoor, the script uses ngrok to expose the local server running on port 80 to the internet. It then prints out the URL where the backdoor can be accessed.

![Screenshot 2024-01-08 12 54 25 AM](https://github.com/CPScript/Saturn/assets/83523587/925a5119-4812-4ebf-b495-a5b4d8eb9960)
