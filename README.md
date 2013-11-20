Gallery CMS
===========

Info
----

GalleryCMS is a free image gallery CMS based on the CodeIgniter 2.1 framework. It is an easy-to-use image gallery CMS that generates JSON and XML feeds that image galleries can consume.

Running on OpenShift
----------------------------

Create an account at http://openshift.redhat.com/ and install the client tools (run 'rhc setup' first)

Create a php-5.3 application (you can call your application whatever you want)

    rhc app create gallerycms php-5.3 mysql-5.1 --from-code=https://github.com/tigefa4u/GalleryCMS

That's it, you can now checkout your application at:

    http://gallerycms-$yournamespace.rhcloud.com

Features
--------

 + Multiple image uploader
 + Drag and drop ordering
 + User management
 + Feed organizer

Dependencies
------------

 + PHP >= 5.2
 + MySQL Database
 + GD2 Library enabled


Installation
------------

1. Create a MySQL database.

2. Edit application/config/database.php and enter your database credentials.

3. Upload to your webserver.

4. Navigate to the URL of which you uploaded the application and complete the registration. Creating your account will generate all of the database tables and finish the installation.


Known Issues
------------

PNG Uploads fail. This is a known CodeIgniter 2.1 issue.