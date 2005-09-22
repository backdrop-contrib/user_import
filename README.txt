********************************************************************
                     D R U P A L    M O D U L E
********************************************************************
Name: user import module
Author: Robert Castelo <services at cortextcommunications dot com>
Drupal: 4.6.x
********************************************************************
DESCRIPTION:

Import users into Drupal from a csv file (comma seperated file).

Features include:

Creates an account for each user.
Match csv columns to profile fields
Can create Usernames based on data from file, e.g. "John" + "Smith" => "JohnSmith".
Usernames can be made of abbreviated data from file, e.g. "John" + "Smith" => "JSmith".
Can create random, human readable, Usernames.
Creates random passwords for each new account.
Can send welcome email, with account details to each new user.
Can set each user's contact form to enabled
Test mode option to check for errors.
Processing can be triggered by cron or manually by an administrator.
Can stagger number of users imported, so that not too many emails are sent at one time.
Multiple files can be imported/tested at the same time.
Designed to be infinitely scalable.



********************************************************************
INSTALLATION:

Note: It is assumed that you have Drupal up and running.  Be sure to
check the Drupal web site if you need assistance.  If you run into
problems, you should always read the INSTALL.txt that comes with the
Drupal package and read the online documentation.

1. Place the entire user_import directory into your Drupal modules/
   directory.
   

2. Load the database definition file.
   
   Create the database tables by using user_import.mysql using the tool of your choice 
   (e.g. phpmyadmin). For mysql and command line access use:

     mysql -u user -p drupal < user_import/user_import.mysql

   Replace 'user' with the MySQL username, and 'drupal' with the
   database being used.

3. Enable the user_import modules by navigating to:

     administer > modules
     
  Click the 'Save configuration' button at the bottom to commit your
  changes.
  
  
********************************************************************
TO DO

  Previous/Next buttons to view more than just the first line of csv file when matching to profile fields.
  Refine text descriptions and help.




