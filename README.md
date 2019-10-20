#The GitDemo

[GitDemo](https://projects.raspberrypi.org/en/projects/getting-started-with-git/6)

Git Commands
git init

Next, you can create a file that will tell people what the project is about. You can use any text editor to do this, such as Notepad, TextEdit or Gedit. Create a file called README.md. The .md extension stands for Markdown, which is a markup language. You can learn more about Markdown here.

You can now give the file a title and write a short explanation of what your project is about.

# The Golden Snitch Sniffer
This is a project that uses multiple long-range ultrasonic sensors to find and track
an object flying in three-dimensional space. It displays the object's coordinates,
speed, and trajectory through a VR headset.
Pressing Ctrl + X will cause a save prompt to appear. You can type Y to save and then hit Enter to close nano.

Your file should have been created and will now be sitting in your directory. You can type ls in the terminal or dir if you are using Windows, to see a list of files.

ls
At the moment, the directory is just like any other directory on your system. You now need to make the magical school bag part. This is known as a Git repository, and it takes the form of a hidden directory that keeps track of all the changes to the working directory. Type the following to create the repository, which from now on will just be called a repo:

git init
If you type ls again, nothing will appear to have changed. You can use ls -a to see all the hidden files and directories, though. If you are using Windows then type dir /A instead.

ls -a
You should now see something like this in your terminal window:

.  ..  .git  README.md
That .git directory is the repo skeleton. You can have a look inside it by typing the following. (Remember if you are using Windows it would be dir /A .git.)

ls -a .git
This should bring up something like:

branches  config  description  HEAD  hooks  info  objects  refs
You don’t really need to worry about this directory at all now. Just know that it is there and that it is tracking all the changes to the parent directory snitch-sniffer.