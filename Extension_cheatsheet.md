
# Carla's Command-Line CheatSheet 

###### 09/08/22

🔑:

>> **** = *Question/command*

**Command Line (CLI)** 

Meaning: The space which the user enters the commands that the computer will process.

**Why use commands?**

May take time to learn initially, but once learnt it will facilitate + is more efficient + powerful when carrying out processes e.g looking for a file on the computer than using a GUI. When we learn how to do these things on CLI, a single process is only needed to be learnt as it can be applied in any environment.

# Navigate The File System





>>				**HOW TO CHECK THE DIRECTORY?** 

**p**rint 
**w**orking 
**d**irectory

By using the **“pwd”** command, you can see in which directory/ folder of the Finder you are in.

**E.g.** of outcome: 

/Users/yourusername

In this case…

/Users/brightnetworktechnologyacademy/





>>			**HOW TO FIND OUT WHAT IS IN OUR CURRENT DIRECTORY?** 

To list all files and folders, use the command **“ls”** .

**E.g.** of outcome:

a list of files and folders will appear


	•	Con = **"ls"** command will not display everything. 
	•	Add a flag to the **“ls”** command to mod its behaviour. 
	
E.g. **“ls -l”** yields extra info about what is in the directory incl, field’s most recent modification date + size.





>>				**HOW TO IDENTIFY A HIDDEN FILE?** 

Hidden files are marked with a dot **“.”** at the beginning of the name + will not be exposed to the user unless they specifically ask to see it.

These hidden files are usually configuration files which affect the way the system runs if modified & have extra protection.





>>				**HOW TO VIEW HIDDEN FILES?** 

Add the **“-a”** flag to the ls command.





>>		**HOW TO VIEW ALL THE DETAILS FOR ALL FILES WITHIN THE CURRENT DIRECTORY?**

Combine the **“-a”** flag with the **“-l”** flag to the **"ls"** command. 

**E.g. “ls -al”**

a list of files and folders including hidden files





>>				**HOW TO MOVE INTO A DIFFERENT DIRECTORY?**

Use the **“cd”** command to Change Directory.

**E.g.** to move to the documents directory of the file system type: cd Documents

	•	The **“~”** symbol will get replaced with the word “documents.





	
>>				**HOW TO GET BACK TO THE HOME DIRECTORY?**

Type **“cd ~”** or cd on its own. If we change directory accidentally we can go back to where we just were using **“ cd -”**

**Simpler Explanation:**

**"cd"** takes us back to our home directory...

**"cd -"** ... and now we're back in Documents!


*Remember: “cd” command can be used to enter through a series of different folders within one command!*

*E.g. If we had a “Coding” folder within our “Documents” folder above, then we could use:*

*cd Documents/Coding*






>>				**HOW TO AUTO COMPLETE COMMANDS ON MAC?**

Use the **“tab”** key to auto complete e.g. cd Doc(press tab), will display **"cd"** Document.

# CREATE FILES + FOLDERS





>>				**HOW CAN I CREATE A NEW DIRECTORY (FOLDER)?**

Command of make directory **“mkdir”.**

**E.g.**

/Users/yourusername/Documents

mkdir my_directory(NAME)

*Remember!!:*

	•	*File names are case-sensitive, but do avoid relying.*

	•	*Spaces are allowed, but difficult to work with. Recommended to use underscore, remove the whitespace or capitalise new words. E.g.* myNewDirectory*

	•	*The dot “.” = A file extension, meaning users can not name a file/directory with that character*

	•	*The forward slash “/”used as the separator in file paths, meaning it can not be used as the name of a file/directory.*

	•	*A directory must have a unique name within its parent directory.*





>>				**WHICH COMMAND TO CREATE A NEW FILE?**

Use the **“touch”** command for this action.

**E.g.**

cd my_directory

touch my_file.txt

*Remember!!: When creating a file using the command line, include the file extension!*
*Examples of file extensions – *

	•	.txt
	•	.pdf
	•	.png
	•	Also possible to create files without any kind of extension.





# OPEN FILES





>>					**HOW DO I OPEN FILES?**

Use the “open” command. This command will use the default program for that type of file to open it in.

E.g. 

“open my_file.txt” will open a text editor

	•To open files using specific programs use the appropriate keyword defined within the program. E.g. To open our text file using the VSCode editor, we would type “code my_file.txt.

# MODIFY FILES + FOLDERS





>>					**HOW TO MOVE A FILE?**

Use the **“mv”** command. This requires 2 pieces of information:

	•	The thing being moved
	•	The place that it will move to 

To move a file back up a level + into our documents for example: 

mv my_picture.png ..

	•	The **“..”** shortcut = The directory above this one
	•	A single dot **“.”** = “this directory”






>>					**HOW TO RENAME A FILE?**

Using the **“mv”** command, provide a filename (without a directory):

**E.g.** 

mv my_photo.png profile_picture.png





>>					**HOW TO COPY A FILE?** 

Similar to moving a file, but use the **“cp”** command. 

*Remember: Provide the path to the thing that we want to copy, then the location to copy it to.

**E.g.** 

**cp profile_picture.png my_directory**





>>			**HOW TO RENAME THE COPY OF THE FILE AS IT IS MOVED?**

Provide a filename in the second path.

To copy an entire directory add the **“-r”** (for recursive) to the **“cp”** command.





>>					**HOW TO DELETE A FILE?**

Use the **“rm”** command to delete a file.
E.g. 

rm profile_picture.png

*Remember: Be extremely careful because when it is gone, it is gone (or take it to a data recovery specialist)!*





>>					**HOW TO DELETE A DIRECTORY?**

Similar method, but add the **“-r”.**

**E.g.** 

rm -r my_directory





>>			**HOW CAN I BYPASS CONFIRMATION WHEN DELETING SOMETHING?**

A confirmation will be prompted usually when something else depends on the thing the user is trying to have deleted.

Add the **“-f”** flag (be sure that you are certain of this action!)

**E.g.**

**"Rm -rf"** command WITH **"r"** flag deletes the directory + skips all the confirmation steps. **"f"** = Force 





>>			**HOW CAN I ADD MULTIPLE DIRECTORIES AT ONCE?**

Use quotation marks **""**, for each directory.

**E.g.**

Within the parent directory the user wants to create a directory (folder) for each day...

: mkdir "Monday" "Tuesday" "Wednesday" "Thur.."


GIT SESSION 

>>					**WHAT IS A GIT**

In Terminal you can use Git to track folders (directories) as a repository (aka Repo)





>>			**HOW DO I CONVERT A LOCAL DIRECTORY INTO A REPOSITORY?**

Run the command **"git init"** to initiate.

*Outcome: Creates a .git folder within the users directory. The .git folder will contain Git records +configoration files. (DO NOT EDIT THOSE FILES DIRECTLY!)





>>			**HOW TO CREATE A NEW COMMIT FROM CHANGES ADDED TO STAGING AREA?**

Run the **"git commit"** command. Mandatory to include a **"-m"** to commit staged files.

**E.g.** git commit -m "..."






>>					**WHAT IS COMMIT?**

Commit acts  as a snap shot of changes made. (AN OBJECT)





>> 			**HOW TO DISPLAY THE STATUS OF YOUR WORKING DIRECTORY?**

Use the command **"git status"**. 





>> 				**HOW CAN I ADD A FILE TO THE STAGING AREA?**

Run **"git add [file]"** *or* dot **"."** for the directory.





>> 				**HOW TO GET CHANGES FROM REMOTE?**

Type **"git pull [remote]"**. This fetches changes from the remote + merges current branch with its upstream.





>> 				**HOW TO REVERT CHANGES MADE TO COMMIT?**

Run the **"git revert [commit sha]"** command to create a new commit, revert changes from specified commit


>>			**HOW TO DOWNLOAD PROJECTS WITH ALL HISTORY FROM REMOTE REPOSITORY?**

Run the command **" git clone [project url or SSH]"**


>> 				**HOW TO UPLOAD REPOSITORIES??????**

**"git push"** , pushes the files to remote repository.
