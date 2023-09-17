<p align="center"> 

<img src="https://i.imgur.com/.png" alt=""/> 

</p> 

<h1>Changing File Permissions in Linux</h1> 

The project will describe the different functions of file permissions by using Linux commands. It will showcase which file permissions need to be provided to employees who need the correct access for a fictitious company, known as Cyber Linxz.
 <br /> 

  

<h2>Items Used</h2> 

  
- Linux

- Linux Commands
   

<h2>Check file and directory details</h2> 
<p> 

<img src="https://imgur.com/uZn9SqU.png" height="80%" width="80%" alt=""/> 

</p> 

<p> 

cd /home/researcher2/projects: this command will open the directory projects. ls -l: this command will list the permissions in the projects directory. 

<h2>Describe the permission string</h2>  
<p>
 <img src="https://imgur.com/DZ7HA0w.png" height="10%" width="10%" alt=""/>
</p>
<p> 

The permissions string incidates which group has a permission. 
- The first character indicates the file type, which the (d) stands for directory. When a hyphen (-) appears it means that it is a regular file. 
- The 2nd - 4th character incidates the read [r], write [w], execute [x] permissions for the User group. When one of the characters is a hyphen (-) it indicates that the permission is not granted 
- The 5th - 7th character indicates the read [r], write [w], execute [x] permissions for the group. 
- The 8th - 10th character incidates the read [r], write [w], execute [x] permissions for the owner type of other. This considers all other types of users in the system separated from the user and group
- The second block of text in the expanded directory listing is the user who owns the file. The third block of text is the group owner of the file.

</p> 

<br /> 

<h2>Change File Permissions</h2> 

<p> 

<img src="https://imgur.com/drYgSel.png" height="80%" width="80%" alt=""/> 

</p> 

<p> 

chmod o-w project_k.txt: this command changes file permissions and removes file permissions from incorrect users and a group. Specifically, the minus (-) is used to remove the writer (w) permission from the others (o). Below the chmod g-w and g-r commands remove the read and write permissions for the group for the file project_m.txt. 

</p> 

<h2>Change file permissions on a hidden file</h2> 

<p> 

<img src="https://imgur.com/WGVEoF3.png" height="80%" width="80%" alt=""/> 

</p> 

<p> 

The command ls -a displays the hidden files in a directory. Below the file .project_x.txt had the incorrect permissions, as the user and the group should only have the read permissions. The write permission was removed from the user and the group. Also, the group was granted access to the read permission by using the chmod command.

</p>

<h2>Change directory permissions</h2> 

<p> 

<img src="https://imgur.com/p8MvuS7.png" height="60%" width="60%" alt=""/> 

</p> 

<p> 

The above shows that the execute permissions for the group of the ‘drafts’ directory were removed. As the owner of the directory, researcher2 should only have the execute permission.

</p> 

<h2>Summary</h2> 

<p> 

In this project, multiple permissions were changed for files and directories. This allowed users, groups, and other users to receive the appropriate permissions. Also, the commands used provided a good demonstration of how to navigate to directories and uncover hidden files. 

</p> 

<br /> 
