# Using FTP for Transferring Files

**Average Reading Time**: 3 minutes

**Difficulty**: Easy to Medium

Is your account's cPanel File Manager inaccessible? Does the File Manager doesn't satifies your needs? Or you want ease the transfer process of the files from your device to the server? 

Then, prepare yourself. In this article, we will be using the FTP method in uploading files as well as managing files in your website.
 
## Getting Started
You need to gather these informations first:

- Your package's FTP account username
- Your package's FTP account password
    
You need all of that for the ftp authentication.
Next, you need to download and install an FTP client. There are many ftp clients to choose from. But solely in this guide, we will use Filezilla. But you can also use any other ftp clients, in any other platforms.
    
### How to Get Your Package's FTP Authentication Details

1. Navigate to your package's cPanel. If you dont know how, see this post.
2. Now, goto to "Files" section. Find and click the "FTP Accounts" option.
3. Choose an FTP Account. If you still haven't created one, see this post.
4. After deciding what FTP account you will use, goto "Actions" and click "Configure FTP Client".
5. A set of details and options can now be seen. Under "Manual Settings", you will see the ftp username, server, and the port.
6. Done. We now got the ftp authentication details. Save these details as we need it later.

### How to Authenticate and Enter FTP

1. Open FileZilla
2. Open File > Site Manager
3. Click New Site
4. In Host, type: **ftp.example.com**, where *example.com* is your website's domain
5. From the Logontype dropdown select "**Normal**"
6. In User, type your ftp account username (eg. *admin@example.com*)
7. In Password, type the password
8. Click OK.

Now, were done saving ftp connection details in our ftp client. You may also want to change alias name of the saved ftp connection "literally aka Site Name" to "yoursite.com" for easy navigation.

9. In "Select Entry", select the site you want to connect.
10. Click Connect

Congrats! You just successfully connected to your package's FTP server. You can now transfer files.

NOTE: If you cant connect or an error has occured, see this post. 

## How to Transfer Files

1. Connect to FTP via FileZilla, if still not, go to the above post.
2. You will now see two views labeled with "Local Site" & "Remote Site". The left side is your device local directory and the right side is your website files.
3. In right side view, navigate and enter to /htdocs.
4. To upload, drag a folder or a file from the left side and drop it to the right.
5. To download, drag a folder from the right side to the target directory of the left side.

### Managing Files in FTP
Now that you have ftp access, you can do most functionalities like what the file manager does. Add, delete, edit, modify your files to suit your needs.
The benefits of using this method are reliability, increase workflows, easy file transfers, and the greater control of file management.
