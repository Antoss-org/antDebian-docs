---
title: 1. Definitions and overview
---

## 1.1. What is this FAQ?

 This document gives frequently asked questions (with their answers!) about the Debian distribution (Debian GNU/Linux and others) and about the Debian project. If applicable, pointers to other documentation will be given: we won't quote large parts of external documentation in this document. You'll find out that some answers assume some knowledge of Unix-like operating systems. We'll try to assume as little prior knowledge as possible: answers to general beginners questions will be kept simple.

If you can't find what you're looking for in this FAQ, be sure to check out Section 12.1, “What other documentation exists on and for a Debian system?”. If even that doesn't help, refer to Section 16.2, “Feedback”.

## 1.2. What is Debian GNU/Linux?

Debian GNU/Linux is a particular distribution of the Linux operating system, and numerous packages that run on it.

Debian GNU/Linux is:

- **full featured**: Debian includes more than 64961 software packages at present. Users can select which packages to install; Debian provides a tool for this purpose. You can find a list and descriptions of the packages currently available in Debian at any of the Debian mirror sites.

    free to use and redistribute: There is no consortium membership or payment required to participate in its distribution and development. All packages that are formally part of Debian GNU/Linux are free to redistribute, usually under terms specified by the GNU General Public License.

    The Debian archives also carry approximately 1082 software packages (in the non-free and contrib sections), which are distributable under specific terms included with each package.

    dynamic: With about 1629 volunteers constantly contributing new and improved code, Debian is evolving rapidly. The archives are updated twice every day.

Most Linux users run a specific distribution of Linux, like Debian GNU/Linux. However, in principle, users could obtain the Linux kernel via the Internet or from elsewhere, and compile it themselves. They could then obtain source code for many applications in the same way, compile the programs, then install them into their systems. For complicated programs, this process can be not only time-consuming but error-prone. To avoid it, users often choose to obtain the operating system and the application packages from one of the Linux distributors. What distinguishes the various Linux distributors are the software, protocols, and practices they use for packaging, installing, and tracking applications packages on users' systems, combined with installation and maintenance tools, documentation, and other services.

Debian GNU/Linux is the result of a volunteer effort to create a free, high-quality Unix-compatible operating system, complete with a suite of applications. The idea of a free Unix-like system originates from the GNU project, and many of the applications that make Debian GNU/Linux so useful were developed by the GNU project.

For Debian, free has the GNUish meaning (see the Debian Free Software Guidelines). When we speak of free software, we are referring to freedom, not price. Free software means that you have the freedom to distribute copies of free software, that you receive source code or can get it if you want it, that you can change the software or use pieces of it in new free programs; and that you know you can do these things.

The Debian Project was created by Ian Murdock in 1993, initially under the sponsorship of the Free Software Foundation's GNU project. Today, Debian's developers think of it as a direct descendent of the GNU project.

Although Debian GNU/Linux itself is free software, it is a base upon which value-added Linux distributions can be built. By providing a reliable, full-featured base system, Debian provides Linux users with increased compatibility, and allows Linux distribution creators to eliminate duplication of effort and focus on the things that make their distribution special. See Section 14.3, “I am making a special Linux distribution for a "vertical market". Can I use Debian GNU/Linux for the guts of a Linux system and add my own applications on top of it?” for more information.
1.3. OK, now I know what Debian is... what is Linux?!

In short, Linux is the kernel of a Unix-like operating system. It was originally designed for 386 (and better) PCs; today Linux also runs on a dozen of other systems. Linux is written by Linus Torvalds and many computer scientists around the world.

Besides its kernel, a "Linux" system usually has:

    a file system that follows the Linux Filesystem Hierarchy Standard https://www.pathname.com/fhs.

    a wide range of Unix utilities, many of which have been developed by the GNU project and the Free Software Foundation.

The combination of the Linux kernel, the file system, the GNU and FSF utilities, and the other utilities are designed to achieve compliance with the POSIX (IEEE 1003.1) standard; see Section 4.4, “How source code compatible is Debian with other Unix systems?”.

For more information about Linux, see What is Linux by Linux Online.
1.4. Does Debian just do GNU/Linux?

Currently, Debian is only available for Linux, but with Debian GNU/Hurd and Debian on BSD kernels, we have started to offer non-Linux-based OSes as a development, server and desktop platform, too. However, these non-linux ports are not officially released yet.

The oldest porting effort is Debian GNU/Hurd.

The Hurd is a set of servers running on top of the GNU Mach microkernel. Together they build the base for the GNU operating system.

Please see https://www.gnu.org/software/hurd for more information about the GNU/Hurd in general, and https://www.debian.org/ports/hurd/ for more information about Debian GNU/Hurd.

A second effort is the port to a BSD kernel. People are working with the FreeBSD kernel.

See https://www.debian.org/ports/#nonlinux for more information about these non-linux ports.
1.5. What is the difference between Debian GNU/Linux and other Linux distributions? Why should I choose Debian over some other distribution?

These key features distinguish Debian from other Linux distributions:

Freedom:

    As stated in the Debian Social Contract, Debian will remain 100% free. Debian is very strict about shipping truly free software. The guidelines used to determine if a work is "free" are provided in The Debian Free Software Guidelines (DFSG).
The Debian package maintenance system:

    The entire system, or any individual component of it, can be upgraded in place without reformatting, without losing custom configuration files, and (in most cases) without rebooting the system. Most Linux distributions available today have some kind of package maintenance system; the Debian package maintenance system is unique and particularly robust (see Chapter 7, Basics of the Debian package management system).
Open development:

    Whereas many other Linux distributions are developed by individuals, small, closed groups, or commercial vendors, Debian is a major Linux distribution that is being developed by an association of individuals who have made common cause to create a free operating system, in the same spirit as Linux and other free software.

    More than 1120 volunteer package maintainers are working on over 64961 packages and improving Debian GNU/Linux. The Debian developers contribute to the project not by writing new applications (in most cases), but by packaging existing software according to the standards of the project, by communicating bug reports to upstream developers, and by providing user support. Additionally, more than 509 volunteer in the project doing other tasks. Examples of these tasks include: creating documentation, contributing to the website translating. See also additional information on how to become a contributor in Chapter 13, Contributing to the Debian Project.
The Universal Operating System:

    Debian comes with more than 64961 packages and runs on 9 architectures. This is far more than is available for any other GNU/Linux distribution. See Section 5.1, “What types of applications and development software are available for Debian GNU/Linux?” for an overview of the provided software and see Section 4.1, “On what hardware architectures/systems does Debian GNU/Linux run?” for a description of the supported hardware platforms.
The Bug Tracking System:

    The geographical dispersion of the Debian developers required sophisticated tools and quick communication of bugs and bug-fixes to accelerate the development of the system. Users are encouraged to send bugs in a formal style, which are quickly accessible by WWW archives or via e-mail. See additional information in this FAQ on the management of the bug log in Section 12.4, “Are there logs of known bugs?”.
The Debian Policy:

    Debian has an extensive specification of our standards of quality, the Debian Policy. This document defines the qualities and standards to which we hold Debian packages.

For additional information about this, please see our web page about reasons to choose Debian.
1.6. How does the Debian project fit in or compare with the Free Software Foundation's GNU project?

The Debian system builds on the ideals of free software first championed by the Free Software Foundation and in particular by Richard Stallman. FSF's powerful system development tools, utilities, and applications are also a key part of the Debian system.

The Debian Project is a separate entity from the FSF, however we communicate regularly and cooperate on various projects. The FSF explicitly requested that we call our system "Debian GNU/Linux", and we are happy to comply with that request.

The FSF's long-standing objective is to develop a new operating system called GNU, based on Hurd. Debian is working with FSF on this system, called Debian GNU/Hurd.
1.7. How does one pronounce Debian and what does this word mean?

The project name is pronounced Deb'-ee-en, with a short e in Deb, and emphasis on the first syllable. This word is a contraction of the names of Debra and Ian Murdock, who founded the project. (Dictionaries seem to offer some ambiguity in the pronunciation of Ian (!), but Ian prefers ee'-en.)