# How to install WordPress on free server

As you may have noticed, Softaculous on free server doesn't have WordPress. Then how do you install it? Here it is.

1. Obtain WordPress from [here](https://wordpress.org/latest.zip) and upload it to your hosting account. *(Make sure you're uploading to public_html directory.)*
2. Open CWP's online file manager and go to public_html folder.
3. Beside WordPress' ZIP file, click decompress from actions menu and click "Decompress File".
4. Once extracted, move all contents of "wordpress" directory back to public_html folder. *(Don't forget to remove "wordpress" folder and WordPress' ZIP file once you done moving.)*
5. Close online file manager, and go to Databases > MySQL Manager from sidebar.
6. Click "Add Database".
7. Name the database with anything you want.
8. In "Select or create a new user", select "Create a new user".
9. Name the user with anything you want, and **Write down your database name, username, and password somewhere safe.**
10. In "Permissions for the user" section, open "Privileges" and check the checkbox in "structure" to grant all user permissions to the database.
11. Click Save.
12. Go back to Online file manager, rename *wp-config-sample.php* to *wp-config.php*, and edit it.
13. Insert your database credentials to *MySQL Settings* section.
14. Go to *Autentication unique keys and salts* section, open new tab, open [this link](https://api.wordpress.org/secret-key/1.1/salt/), copy all of it's contents, and paste it to that section, replacing default values.
15. Paste this:
~~~
define('FS_METHOD', 'direct');
~~~
to the bottom of *wp-config.php* file, to make sure you're not asked for FTP credentials everytime you're updating WordPress or installing plugin/theme.

16. Save and close the file, and close online file manager.
17. Open your website and complete installation through web interface.
