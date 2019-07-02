---
id: install-onlyoffice-on-ubuntu1804
summary: Learn 2 alternative ways to install ONLYOFFICE on Ubuntu 18.04 using provided script.
categories: server
tags: ONLYOFFICE, ONLYOFFICE Community Edition
difficulty: 2
status: draft
feedback_url: https://github.com/canonical-websites/tutorials.ubuntu.com/issues
published: 2019-07-03
author: Maria Pashkina <maria.pashkina@gmail.com>

---
# How to Install ONLYOFFICE on Ubuntu 18.04

## INTRODUCTION
Duration: 2:00

[ONLYOFFICE](https://www.onlyoffice.com/en/) is an open source office suite that includes online editors and the range of productivity and collaboration tools such as, documents and projects management, CRM system and calendar, chat and email, all in one place.

ONLYOFFICE Community Edition, distributed under GNU AGPL v.3,  is composed of three servers:

* Document Server  comprises online editors for text documents, spreadsheets and presentations. You can create, edit and collaborate on documents 100% compatible with MS Office and other popular formats in a familiar tabbed interface. 
* Community Server includes the following modules and tools: People, Projects, CRM, Documents, CRM, Community, mail client, calendar and chat. To learn more about the latest features in Community Server, please, refer to [the official documentation](https://helpcenter.onlyoffice.com/server/community/changelog.aspx).
* Mail Server allows to connect your own domains and create corporate mailboxes.

**WHAT YOU’LL LEARN**

In this tutorial, you will learn two alternative ways to install ONLYOFFICE on Ubuntu 18.04 using the provided script:
* installing Community Edition with a Docker image,
* installing Community Edition from the DEB package. 

**WHAT YOU’LL NEED**
* System requirements:
CPU: dual core 2 GHz or better
RAM: 6 GB or more
HDD: at least 40 GB of free space
* Additional requirements: at least 6 GB of swap
* Software requirements: Ubuntu 18.04
* Installation with a docker: Docker: version 1.10 or later
* Administrative permissions for program installation

---
## INSTALLATION 
Duration: 10:00

**1. Get Community Edition script**

Download ONLYOFFICE script file using the direct link:
```sh       
$ wget http://download.onlyoffice.com/install/opensource-install.sh
```
**2. Running Community Edition Installation**
Please note that to perform  all  installation  actions you must be logged in with root rights.

**2.1** Run the complete ONLYOFFICE installation:
```sh
$ bash opensource-install.sh -md "yourdomain.com"
```
Specify your registered domain name instead of  "yourdomain.com".

In case you don’t want or don’t need to install Mail Server, run the following command:
```sh
$ bash opensource-install.sh -ims false
```
**2.2** After you have initiated running a script, you will have to choose one of the installation options depending on your needs:

Install with Docker [Y/N/C]?

* Select 'Y' to install ONLYOFFICE using Docker.

This option is recommended, if you want to install Community Edition including Community, Document and Mail servers at once. Docker script will set up Docker containers with all the modules and dependencies necessary for Community Edition correct work and is easy to run, manage and update.

* Select 'N' to install it using DEB package.

The script will automatically install and configure all the necessary prerequisites as well as Community Edition components (Document Server and Community Server). Please note, that in case you select DEB installation, you will need to manually install Mail Server and  connect it to your ONLYOFFICE installation. See instructions in [our Help Center](https://helpcenter.onlyoffice.com/server/docker/mail/connect-mail-server-to-community-server-via-portal-settings.aspx).

---

## INSTALLATION COMPLETE

After installation is over, check Community Edition for correct work.

![](https://personal.onlyoffice.com/products/files/httphandlers/filehandler.ashx?action=download&fileid=2992962&doc=YU12cDRXNGowYmZVTzJnM1Y0R0ZVVjFya3BEOW5nVXQ4Q3VFRVI3RmdkQT0_IjI5OTI5NjIi0)

Once completed, specify your email and create a password to access your web office next time.

Well done! You have successfully installed ONLYOFFICE. Now you have at your disposal a full-featured online collaboration platform for your team:

* create, edit and collaborate on your office documents of different formats from anywhere at any time. You can also work with your documents offline using ONLYOFFICE Desktop Editors connected to your portal. To learn more, please refer to [this tutorial](https://tutorials.ubuntu.com/tutorial/install-onlyoffice-desktop-editors-on-ubuntu1804#0.).

![](https://personal.onlyoffice.com/products/files/httphandlers/filehandler.ashx?action=download&fileid=2992991&doc=YnNzb2NwTHRkMXRzTVNZVEF3Tmd4YW5aZ3l0VElTSU5RTDlFeTFQOGc5Yz0_IjI5OTI5OTEi0)

* store and manage all the documents, including the files from the cloud storage services like Google Drive, Dropbox, ownCloud. Share your files with different access permissions. Store and play video and music, view images of all popular formats: BMP, JPG, JPEG, PNG, GIF, TIF, TIFF, AVI, MPEG, MP3, PDF, etc. with integrated multi-format media player.

![](https://personal.onlyoffice.com/products/files/httphandlers/filehandler.ashx?action=download&fileid=2992998&doc=aHpYY0xaQUJZNmQzQVdIVEVYNFQ0d3djemQwZVdQUkIyVUJSR1ZYU2xCRT0_IjI5OTI5OTgi0) 

* carry out the project through all its stages: schedule workflow, distribute tasks and subtasks, store the project related documentation, lead discussions, track time, generate reports via docbuilder.

![](https://personal.onlyoffice.com/products/files/httphandlers/filehandler.ashx?action=download&fileid=2993010&doc=WmxQZ2wyMmlwRGpsWjdqbzdyV1B5NnBpTmZtcWw3K0k4YUpVWmRuVHJGbz0_IjI5OTMwMTAi0)

* create a client database and keep track of the potential sales via CRM module.

![](https://personal.onlyoffice.com/products/files/httphandlers/filehandler.ashx?action=download&fileid=2993016&doc=UXBlSm15eEE1RnZxRmpvdlFlZEl4V0JoM2d1K3lIbVh0VGgzcVZYekhudz0_IjI5OTMwMTYi0)

* organize an internal social network with news, blogs, forums, bookmarks, polls, wiki.

![](https://personal.onlyoffice.com/products/files/httphandlers/filehandler.ashx?action=download&fileid=2993023&doc=MlBNM0xsbXNtTEp4a2NhektSTFp3V2IyRnNqbHEvZ1hTUFZnbEF1MDdiQT0_IjI5OTMwMjMi0)

* manage all your email efficiently in module Mail: connect different email accounts and manage all the correspondence from one single place and create corporate mailboxes for your team members.

![](https://personal.onlyoffice.com/products/files/httphandlers/filehandler.ashx?action=download&fileid=2993035&doc=WWUwZ3UreE1WSjJhYmgxaGZQNVh3NmxOOTZrdktZdlAxVk01dlR2ajN6az0_IjI5OTMwMzUi0)

* schedule corporate and personal events using Calendar that can be integrated with other modules and synchronized with third part apps.

![](https://personal.onlyoffice.com/products/files/httphandlers/filehandler.ashx?action=download&fileid=2993048&doc=V0x2dWVVSktTTGFyaWZGaExQdTBSS3NEVXVlcEZLWnhzdnI0bG8ydGJzTT0_IjI5OTMwNDgi0)

Select the tool you need and start working. Enjoy!

