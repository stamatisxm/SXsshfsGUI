# SXsshfsGUI
Zenity-driven Mount / Unmount of remote directories via sshfs

<img alt="SXencGUI Logo" src="http://ideaware.xyz/wp-content/uploads/2017/07/SXsshfsGUI.png" width="48px" height="48px" />

## SXsshfsGUI – { Mount / Unmount Remote Directories via sshfs }
SXsshfsGUI is a simple Zenity front-end to sshfs, useful for handling the mounting / unmounting of remote directories via sshfs. The interface is simple and self explanatory.

### { Program Options }

This is the interface of SXsshfsGUI:

<img alt="SXencGUI Interface" src="http://ideaware.xyz/wp-content/uploads/2017/07/SXsshfsGUI-SShot.png" />

The “Action” is a drop-down that contains the **Mount**, **Unmount** and **Refresh** options.

To mount a remote directory, select **Mount** from the **Action** menu and either type the path manually into the “Remote Directory” text field, or select a predefined (see below)* path from the “Remote Directory” dropdown menu, follow the **Directory Selection Dialog** to choose the **mount point**, enter your **password** for the remote machine and click **OK**


#### * Predefined remote paths
These can be contained (one path per line) in a file named **.SXsshfsGUIrc** in the user's **$HOME** directory and will be of the format:

**server:"remote_path_to_be_mounted"**

[Note that the quotes are optional]


The “Mounted Directories” box displays a list of the mountpoints currently used.

To unmount a remote directory, select **Unmount** from the **Action** menu, select the directory from the “Mounted Directories” List and click on the “Mount/Unmount/Refresh” button.

Lastly, there is a help drop-down menu, labelled “Click drop-down Help”, summarizing the program’s operation.

### { Program Setup }
This program is going to be installed by default in your **$HOME/bin** directory. If you have not set your **$HOME/bin** in the **$PATH**, see [this](http://istos.xyz/linux/include-homebin-in-any-desktop-environment/ "Include $HOME/bin in any Desktop Environment") or [this snippet](http://istos.xyz/linux/include-homebin-in-the-path-for-bash-shell "Setup your $HOME/bin in the $PATH") for details.

To run this program, you need to have the following packages installed in your system (Check with your package manager):

- _**zenity**_
- _**sshfs**_

#### Once the above packages are installed
- Download SXsshfsGUI
- Move the downloaded tarball into your **$HOME**, as all extracted files and directories will be relative to your **$HOME**
- Expand the tar file in a terminal by issuing:  
<code>**tar xf SXsshfsGUI\_&lt;version&gt;.tar**</code>
- Invoke the program from the terminal, running:  
<code>**SXsshfsGUI &**</code>  
to ensure that it loads properly and no error messages are shown.

If everything has gone ok, you should be able to find the program in the _**Accessories**_ program group on your desktop manager.

### { File List }
The tarball contains these files (relative to the user's $HOME):
<pre>
bin/SXsshfsGUI
.local/share/icons/SXsshfsGUI.png
.local/share/applications/SXsshfsGUI.desktop
</pre>

