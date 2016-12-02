## Introduction
International in scope and free for public use, OVAL is an information security community effort to standardize how to assess and report upon the machine state of computer systems. OVAL includes a language to encode system details, and an assortment of content repositories held throughout the community.

This GitHub project hosts the OVAL Language Schemas and Specifications to improve transparency and the community's ability to track changes before a release. As of the OVAL 5.11.1 release, releases of the OVAL Language will no longer be posted on the OVAL Web Site, rather, here on this GitHub project.

Development: [OVAL 5.11.1] (https://github.com/OVALProject/Language)<br>
Official: [OVAL 5.11.1] (https://github.com/OVALProject/Language/wiki/Latest)<br>
Previous: [OVAL Archives] (http://oval.mitre.org/archive)<br>

Experimental capabilities for the OVAL Language will be developed in the [OVAL Language Sandbox] (http://oval.mitre.org/language/sandbox.html) to allow the community to fully investigate and implement new capabilities before they are included here in an official release ensuring that only mature and implementable constructs are added to the OVAL Language.

## Developing an Official OVAL Language Release
The process of developing an official OVAL Language release is outlined in the [OVAL Language Revision Process] (http://oval.mitre.org/language/about/revision_process.html) and follows the [OVAL Language Versioning Policy] (http://ovalproject.github.io/documentation/policy/versioning/).

## OVAL Language Naming and Design Conventions
OVAL Language naming and design conventions can be found in the [OVAL Developer's Guide](http://ovalproject.github.io/getting-started/best-practices/)

## Quick Start Guide
1. Set up [Git](http://help.github.com/win-set-up-git/) on your system
2. Create a new [issue](https://github.com/blog/831-issues-2-0-the-next-generation) to request a new feature or to report a bug in the [OVAL Language Tracker](https://github.com/OVALProject/Language/issues)
3. [Fork](http://help.github.com/fork-a-repo/) the OVAL Language Repository
4. [[Make changes|Make Changes]] to your fork
5. Send a [pull request](http://help.github.com/send-pull-requests)
6. [Sync] (https://help.github.com/articles/syncing-a-fork) your fork to get the latest changes

## Retrieving a Specific Revision
During the development of an OVAL Language release, the specifications will go through many draft revisions and potentially multiple release candidate revisions before becoming official. Each revision of the OVAL Language, will be tagged with a [Git tag] (http://git-scm.com/book/en/Git-Basics-Tagging) to save the changes at that point in time for review in the future.

Tag naming conventions:<br>

    Draft:     
     <revision>-draft-<draft-number> (e.g. 5.11-draft-1)

    Release Candidate:      
     <revision>-rc-<rc-number> (e.g. 5.11-rc-1)
  
    Official: 
     <revision> (e.g. 5.11)

List the available revision tags:<br>

    git tag -l

Get a specific revision tag:<br>

    git checkout <revision-tag>

Alternatively, you may retrieve a specific revision through the GitHub project page.

1. Navigate to the [OVAL Language GitHub Project](https://github.com/OVALProject/Language)
2. Click the _Switch branch/tag_ drop-down box (immediately to the left of the _Files_ tab)
3. Select the _Tags_ tab
4. Select the desired tag
5. Click the _ZIP_ button

## Verifying a Tag
To verify a tag, you will first need to import our public key into your key ring. Our public key is:

    oval-public-key (coming soon)

Import our public key:

     gpg --import oval-public-key.gpg

Once imported, you can verify the tag:

    git tag -v <revision-tag>

## Viewing the Changes Between Revisions
As new revisions are published, it will be useful to track the changes from one revision to the next.

To view the statistics of the changes between two revisions:

    git diff <revision-1> <revision-2> --stat

To view a diff of all changes between two revisions:

    git diff <revision-1> <revision-2>

To view a diff of all changes, for a particular set of files, between two revisions:

    git diff <revision-1> <revision-2> -- <filename1> [<file-2> <file-3> ...]

You may also view the differences between revisions through the GitHub project page.

1. Navigate to the [OVAL Language GitHub Project](https://github.com/OVALProject/Language)
2. Click the _Switch branch/tag_ drop-down box (immediately to the left of the _Files_ tab)
3. Select the _Tags_ tab
4. Select the desired tag
5. Click the file that you would like to view the history of
6. Click the _History_ button
7. Select the commit that you are interested in to see the diff

## Requesting a New Feature, Reporting a Bug, or Getting Help
If you would like to request a new feature or report a bug, please create a new [issue](https://github.com/blog/831-issues-2-0-the-next-generation) in the [OVAL Language Tracker](https://github.com/OVALProject/Language/issues). 

Please send all help requests to the oval-developer-list by sending a message to oval_developer@lists.cisecurity.org. You may also request new features or report bugs by sending a message to this mailing list. If you are not currently subscribed to this mailing list, you may sign up at https://oval.cisecurity.org/community/discuss.

## Useful Links
The [[Useful Links]] page contains links to resources that will help with the OVAL Language and GitHub among other things.