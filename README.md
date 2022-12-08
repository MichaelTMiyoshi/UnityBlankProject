# UnityBlankProject
 
This is a blank Unity project that can be cloned/forked for a starting point.

The biggest lesson when creating a Unity project is to make sure that the .gitignore is set up correctly.  The .gitignore at the [link](https://www.toptal.com/developers/gitignore/api/unity) is a good starting point.  It is not much different than the one created by GitHub Desktop when you select Unity.  I also added the .DS_Store at the bottom of the file because I am usually doing Unity on a Mac.

The biggest thing to note though is that the .gitignore file needs to be in the Unity project folder.  When you create it at first, it will go into the repository.  But it does not seem to work unless it is in the project folder.  So I have kept it in both places.  I thought it was supposed to propagate downward through the directories, but this does not seem to be the case.  So just put the .gitignore file into the Unity project folder.

By the way.  I had a couple missteps along the way to making this blank Unity project repo.  I ended up needing to use 

```git reset --hard HEAD^```

(from terminal) a couple times because github desktop wanted to sync all the files in the project even though I was trying to tell it not to with the .gitignore.  This misstep helped me realize what I had seen somebody else do.  I could take the project folder and move it around.  So I took the project folder out of the local repository folder, copied the .gitignore file to that folder.  Then, I used the git reset command to get back to the empty (or nearly empty repository).  Then, I moved the Unity project folder back into the local repo, commited the changes, then pushed.  It worked like a champ.

So remember.  Put the .gitignore file into the Unity project folder.  That is the key.  (Oh and put the folder into the repository after you do that.)
