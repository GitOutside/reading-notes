## Links
use  ```<a>```. Anything between the opening and closing tags can be clicked on.
```<a href="link URL">TEXT USER CLICKS ON</a>```
 - use descriptive text for link. Be specific so when user is looking for page they are linking to, they can find it more easily
 - make links clearly visible

**href** attribute is assigned value of URL for link
  - Can be absolute (on web) or relative (within site) URL

## Directory Structure
**root folder** - top level folder. All other files and folders for site here
home page for entire sie is in index.html in root folder and that is the default if no file name is specified in URL

**URL frelative links types**
 - same folder:  ***file name***
 - child folder: ***child folder name/ file name***
 - grandchild folder: ***child folder name/grandchild folder name/file name***
 - parent folder: ***../file name***
 - grandparent folder: ***../../file name***
 
 ### ```<a>``` attributes
**href = "mailto:abc@example.com"** for use in ```<a>```to send email to link address
**target** opens the link in a new window. target="_blank". Avoid opening in new window, but if you do, inform user

to link to a spot on the same page, assign id to tag where link will go. Then in ```<a>``` tag, **href** will be assigned to the id for that spot.
```<a href="URL#id></a>

to link to a spot on another page, 
