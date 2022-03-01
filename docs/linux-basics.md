# Operating Systems
{: style="border-bottom: none;margin-bottom:0"}

### Linux Basics
{: style="margin-top:0"}
[Home](https://noahkirchner.github.io/Primers/) | [Github](https://github.com/NoahKirchner/Primers)
## Overview

Linux is one of the big three competing operating systems, and is the latest and most direct competitor
to Windows. While most common distributions of Linux have graphical user interfaces and can be used
for personal or casual usage, it is most commonly seen powering servers and dedicated workstations
for more complex computer science tasks.


More accurately Linux is not an operating system at all. It is a kernel, the piece of software that
connects applications to hardware. On top of the Linux kernel, there is a collection of free software
called GNU. GNU is a software suite that gives most of the functionality to Linux distributions. GNU and
the Linux kernel work together in a pair to produce an operating system.


### Distributions


There are many different versions of operating system that utilize GNU software and the Linux kernel. These
versions are called distributions. While some are created to fulfill a specific purpose, most of them 
follow the same general structure and idea. The vast majority of Linux distributions can be used
as general purpose operating systems and will handle most daily requirements.



Ubuntu, and most modern popular distributions of Linux meant for users instead of industry usage
are derived from Debian. Debian based distributions use command syntax based around the "-" key,
tend to have far more packages (applications) for use, and are more frequently updated. Redhat,
and its free cousin Fedora, have significantly less support than Debian. Redhat's development team,
however, is a company as opposed to an open source community. This means that Redhat updates have the 
potential to be more focused and of better quality. Redhat also has a professional support team for those
who are willing to pay for it, making it useful for professional applications.



This distinction, while it is important to understan if you ever decide to use Linux personally, is
outside of the scope of this document. As such, it will be exclusively focusing on Debian based distributions
from here on as they are the more common of the two types.



### File Structure and Hierarchy


Basic Linux file structure is fairly similar to Windows. Directories contain other directories and files,
and these together create the file hierarchy of the operating system. If you can navigate Windows comfortably,
Linux should not present too much of a problem. There are significant differences in how they are
structured, but for basic usage the general concepts are the same.



The top level directory in Linux is called root. All files and directories are located under this top level.
In Linux, **all** files and directories, to include additional drives, will fall under the root directory.



File paths in Linux take a different form and format than in Windows. Whereas in Windows a file path
looks like:

```C:\Users\Jeffrey```

A Linux filepath uses forward slashes instead of backward slashes to denote directories, like:

```/home/jeffrey```

Linux filepaths are also case sensitive, contrarily to Windows.











---
Noah Kirchner
