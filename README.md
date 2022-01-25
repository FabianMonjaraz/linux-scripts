<H2>BM</h2>
<p>
bm [OPERATION] [PARAMETERS]

Script to create, modificate, delete and view bookmarks in bash.
Once created, they can be accessed via "cd @NAME_OF_BOOKMARK"
At this day, the "alias cd='cd -P'" cannot be setted correctly from
this script, so is adviced to create this alias to show a correct 
format from commands like "pwd"

OPERATIONS 
  This script accept only ONE operation
  -d BOOKMARK_NAME 
    Deletes the bookmark BOOKMARK

  -h Show this message

  -l  List the bookmarks along their real path

  -e OLD_BM_NAME NEW_BM_NAME
    Changes the name of OLD_BM_NAME to NEW_BM_NAME
  
  -m BOOKMARK_NAME
    Create a bookmark of the current directory

  -n PATH BOOKMARK_NAME
    Create a new bookmark

FILES AND VARS
  
  ~/.bashmarks
    The bookmarks are stored here, in the form of symlinks

  CDPATH=$CDPATH:~/.bashmarks
    If this variable is not setted, the script sets it in .bashrc
    </p>
