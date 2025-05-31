---
title: The Debian GNU/Linux FAQ
---

The Debian GNU/Linux FAQ

Version 12.1

Copyright © 1996-2024 Software in the Public Interest

Permission is granted to make and distribute verbatim copies of this document provided the copyright notice and this permission notice are preserved on all copies.

Permission is granted to copy and distribute modified versions of this document under the conditions for verbatim copying, provided that the entire resulting derived work is distributed under the terms of a permission notice identical to this one.

Permission is granted to copy and distribute translations of this document into another language, under the above conditions for modified versions, except that this permission notice may be included in translations approved by the Free Software Foundation instead of in the original English.

October 2024

Abstract

This document answers questions frequently asked about Debian GNU/Linux.

Table of Contents

1. Definitions and overview

    1.1. What is this FAQ?
    1.2. What is Debian GNU/Linux?
    1.3. OK, now I know what Debian is... what is Linux?!
    1.4. Does Debian just do GNU/Linux?
    1.5. What is the difference between Debian GNU/Linux and other Linux distributions? Why should I choose Debian over some other distribution?
    1.6. How does the Debian project fit in or compare with the Free Software Foundation's GNU project?
    1.7. How does one pronounce Debian and what does this word mean?

2. Getting and installing Debian GNU/Linux

    2.1. What is the latest version of Debian?
    2.2. Are there package upgrades in "stable"?
    2.3. Where/how can I get the Debian installation images?
    2.4. How do I install Debian from CD-ROMs?
    2.5. Why does the official stable released CD-ROM contain symlinks for "frozen" and "unstable"? I thought this CD contains just "stable"!
    2.6. Can I get and install Debian directly from a remote Internet site?
    2.7. Are there any alternative strategies for booting the system installer?

3. Choosing a Debian distribution

    3.1. Which Debian distribution (stable/testing/unstable) is better for me?

        3.1.1. You asked me to install stable, but in stable so and so hardware is not detected/working. What should I do?
        3.1.2. Will there be different versions of packages in different distributions?
        3.1.3. The stable distributions really contains outdated packages. Just look at Kde, Gnome, Xorg or even the kernel. They are very old. Why is it so?
        3.1.4. If I were to decide to change to another distribution, can I do that?
        3.1.5. Could you tell me whether to install stable, testing or unstable?
        3.1.6. You are talking about testing being broken. What do you mean by that?
        3.1.7. Why is it that testing could be broken for months? Won't the fixes introduced in unstable flow directly down into testing?
        3.1.8. From an administrator's point of view, which distribution requires more attention?
        3.1.9. What happens when a new release is made?
        3.1.10. I have a working Desktop/cluster with Debian installed. How do I know which distribution I am running?
        3.1.11. I am currently using the stable version. Can I change to testing or unstable? If so, how?
        3.1.12. I am currently tracking testing (trixie). What will happen when a release is made? Will I still be tracking testing or will my machine be running the new stable distribution?
        3.1.13. I am still confused. What did you say I should install?

    3.2. But what about Kali, Knoppix, Linux Mint, Ubuntu, and others?

        3.2.1. I know that Kali/Knoppix/Linux Mint/Ubuntu/... is Debian-based. So after installing it on the hard disk, can I use 'apt' package tools on it?
        3.2.2. I installed Kali/Knoppix/Linux Mint/Ubuntu/... on my hard disk. Now I have a problem. What should I do?
        3.2.3. I'm using Kali/Knoppix/Linux Mint/Ubuntu/... and now I want to use Debian. How do I migrate?

4. Compatibility issues

    4.1. On what hardware architectures/systems does Debian GNU/Linux run?
    4.2. What kernels does Debian GNU/Linux run?
    4.3. How compatible is Debian with other distributions of Linux?
    4.4. How source code compatible is Debian with other Unix systems?
    4.5. Can I use Debian packages (".deb" files) on my Red Hat/Slackware/... Linux system? Can I use Red Hat packages (".rpm" files) on my Debian GNU/Linux system?
    4.6. How should I install a non-Debian program?

5. Software available in the Debian system

    5.1. What types of applications and development software are available for Debian GNU/Linux?
    5.2. Who wrote all that software?
    5.3. How can I get a current list of programs that have been packaged for Debian?
    5.4. How can I install a developer's environment to build packages?
    5.5. What is missing from Debian GNU/Linux?
    5.6. Why do I get "ld: cannot find -lfoo" messages when compiling programs? Why aren't there any libfoo.so files in Debian library packages?
    5.7. (How) Does Debian support Java?
    5.8. How can I check that I am using a Debian system, and what version it is?
    5.9. How does Debian support non-English languages?
    5.10. Where is ezmlm/djbdns/qmail?
    5.11. Where is a player for Flash (SWF)?
    5.12. Where is Google Earth?
    5.13. Where is VoIP software?
    5.14. I have a device that requires non-free firmware. What should I do?
    5.15. I have a wireless network card which doesn't work with Linux. What should I do?

6. The Debian archives

    6.1. How many Debian distributions are there?
    6.2. What are all those names like etch, lenny, etc.?

        6.2.1. Which other codenames have been used in the past?
        6.2.2. Where do these codenames come from?

    6.3. What about "sid"?
    6.4. What does the stable directory contain?
    6.5. What does the testing distribution contain?

        6.5.1. What about "testing"? How is it "frozen"?

    6.6. What does the unstable distribution contain?
    6.7. What are all those directories at the Debian archives?
    6.8. What are all those directories inside dists/stable/main?
    6.9. Where is the source code?
    6.10. What's in the pool directory?
    6.11. What is "incoming"?
    6.12. Where can I find old packages of previous releases?
    6.13. How do I set up my own apt-able repository?

7. Basics of the Debian package management system

    7.1. What is a Debian package?
    7.2. What is the format of a Debian binary package?
    7.3. Why are Debian package file names so long?
    7.4. What is a Debian control file?
    7.5. What is a Debian conffile?
    7.6. What is a Debian preinst, postinst, prerm, and postrm script?
    7.7. What is an Essential, Required, Important, Standard, Optional, or Extra package?
    7.8. What is a Virtual Package?
    7.9. What is meant by saying that a package Depends, Recommends, Suggests, Conflicts, Replaces, Breaks or Provides another package?
    7.10. What is meant by Pre-Depends?
    7.11. What is meant by unknown, install, remove, purge and hold in the package status?
    7.12. How do I put a package on hold?
    7.13. How do I install a source package?
    7.14. How do I build binary packages from a source package?
    7.15. How do I create Debian packages myself?

8. The Debian package management tools

    8.1. What programs does Debian provide for managing its packages?

        8.1.1. dpkg
        8.1.2. APT
        8.1.3. aptitude
        8.1.4. synaptic
        8.1.5. tasksel
        8.1.6. Other package management tools

    8.2. Debian claims to be able to update a running program; how is this accomplished?
    8.3. How can I tell what packages are already installed on a Debian system?
    8.4. How do I display the files of an installed package?
    8.5. How can I find out what package produced a particular file?
    8.6. Why is "foo-data" not removed when I uninstall "foo"? How do I make sure old unused library-packages get purged?

9. Keeping your Debian system up-to-date

    9.1. How can I keep my Debian system current?

        9.1.1. aptitude
        9.1.2. apt-get and apt-cdrom

    9.2. Must I go into single user mode in order to upgrade a package?
    9.3. Do I have to keep all those .deb archive files on my disk?
    9.4. How can I keep a log of the packages I added to the system? I'd like to know when upgrades and removals have occurred and on which packages!
    9.5. Can I automatically update the system?
    9.6. I have several machines; how can I download the updates only one time?

10. Debian and the kernel

    10.1. Can I install and compile a kernel without some Debian-specific tweaking?
    10.2. What tools does Debian provide to build custom kernels?
    10.3. What special provisions does Debian provide to deal with modules?
    10.4. Can I safely de-install an old kernel package, and if so, how?
    10.5. Where can I get more information about Linux packages for Debian?

11. Customizing your Debian GNU/Linux system

    11.1. How can I ensure that all programs use the same paper size?
    11.2. How can I provide access to hardware peripherals, without compromising security?
    11.3. How do I load a console font on startup the Debian way?
    11.4. How can I configure an X11 program's application defaults?
    11.5. How does a Debian system boot?
    11.6. And how about Debian and traditional System V init?
    11.7. And are there yet other ways of booting a Debian system?
    11.8. How does the package management system deal with packages that contain configuration files for other packages?
    11.9. How do I override a file installed by a package, so that a different version can be used instead?
    11.10. How can I have my locally-built package included in the list of available packages that the package management system knows about?
    11.11. Some users like mawk, others like gawk; some like vim, others like elvis; some like trn, others like tin; how does Debian support diversity?

12. Getting support for Debian GNU/Linux

    12.1. What other documentation exists on and for a Debian system?
    12.2. Are there any on-line resources for discussing Debian?

        12.2.1. Mailing lists
        12.2.2. Web forum
        12.2.3. Wiki
        12.2.4. Maintainers
        12.2.5. Usenet newsgroups

    12.3. Is there a quick way to search for information on Debian GNU/Linux?
    12.4. Are there logs of known bugs?
    12.5. How do I report a bug in Debian?

13. Contributing to the Debian Project

    13.1. How can I become a Debian member/Debian developer?
    13.2. How can I contribute resources to the Debian project?
    13.3. How can I contribute financially to the Debian project?

        13.3.1. Software in the Public Interest
        13.3.2. Other organizations

14. Redistributing Debian GNU/Linux in a commercial product

    14.1. Can I make and sell Debian CDs?
    14.2. Can Debian be packaged with non-free software?
    14.3. I am making a special Linux distribution for a "vertical market". Can I use Debian GNU/Linux for the guts of a Linux system and add my own applications on top of it?
    14.4. Can I put my commercial program in a Debian "package" so that it installs effortlessly on any Debian system?

15. Changes expected in the next major release of Debian

    15.1. Hardening the system
    15.2. Extended support for non-English users
    15.3. Improvements in the Debian Installer
    15.4. More architectures
    15.5. More kernels

16. General information about the FAQ

    16.1. Authors
    16.2. Feedback
    16.3. Availability
    16.4. Document format