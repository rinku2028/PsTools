# PsTools
PsTools For System Adminsitrators


PsTools are for both hackers and System Admins. These tools are free to use.

Some of the PsTools command used for command line:

1. psexec
The tool psexec is used to remotely execute programs on a computer. I have used this in the past to execute programs that I installed in an alternate data stream. Quite often when and if a hacker is able to gain access to one of the computers on the network that you work on, you will see psexec transferred over. Back when I wrote the above linked article psexec worked wonderfully well. Now that I am writing about it in this article there are some really odd quirks. It did not want to work and I had to spend an hour or so to try and figure out what went wrong. Well long story short I was able to get it working, but with a different syntax than in the article noted above. On that note, if any of you can tell me what is different here I would be most interested in knowing. With that said let's take a look at how to use psexec via a reverse shell as supplied by Metasploit.

2. psfile
This tool will allow you to see what files are opened remotely on the computer that you invoke this program on locally. By that I mean, if you invoke psfile on say 192.168.1.100 it will show you what files on 192.168.1.100 are presently being viewed by remote computers. It will not however show you the IP address of the computer which has remotely opened a file on your local computer. What it will allow you to do is close the file that is being viewed remotely if you so choose. That is a rather handy feature to have. Seeing is believing, so let's take a look at what the tool looks like when invoked.

3. psgetsid
This tool will allow you to query a computer for its SID. This is rather handy to have unless you wish to go muck about in the registry where most people are loathe to go. This tool will also allow you to not only see a computer's SID, it will also allow you to specify an account name as well.

4. psinfo
One of the best tools in the PsTools suite is psinfo. This little program will give you a list of most of the information that you would ever require. Specific examples of that would be the computer's uptime. A computer's uptime is really rather important as that could indicate if a computer has had a specific patch applied to it or not. If it has not then that computer would be ripe for exploitation via a specific vector. For example, a new remote code execution has been released for Microsoft Windows. Microsoft issued a patch for it two days ago. The computer uptime listed on this computer is four days however. That information would allow you to know that the computer was vulnerable to that exploit. 
