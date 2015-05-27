# 4d-vc-git-v14
## Description
The 4D_VC_GIT Component extends the [VC_Framework](https://github.com/4D/vc-framework-v14 "VC_Framework_V14") component
to provide GIT version control support to 4D V14. This Component is inspired from the 
[VC_SVN](https://github.com/4D/vc-svn-v14 "VC_SVN_V14") Component. In addition, it supports **importing** pulled code back to 4D, 
inspired from [Elutz](https://github.com/elutz "Elutz Profile")'s 
[VC_Import](https://github.com/elutz/vc-framework-v13/blob/master/matrix/VC_Framework.4dbase/vc_source/VC_Import.txt "VC_Import Method") method. 
This way, you can have your team's commits inside 4D. 


## How It Works
* 4D methods are nested inside the .4DB file. It is therefore impossible to Version Control your code. 
* The VC_Framework component creates txt files for the methods & the forms of your 4D project and saves your changes constantly
in these txt files. Making it possible to use a version control system.
* You can then use git CLI tool to commit your changes, push, pull, ...
* When you need to import your team's changes pulled from central repository back to 4D, just Run the **VC_GIT_IMPORT** method. And you're set !


## Important !
The 4D_VC_GIT Component depends on these components :
* [VC_Framework_v14](https://github.com/4D/vc-framework-v14 "VC_Framework_V14")
* [Prog_v14](https://github.com/4D/prog-v14 "Progressbars")

So don't forget to add them to your Components folder.


## Notes
Support for VC_Framework DEVHOOK methods will be added soon :

* VC_DEVHOOK_Create
* VC_DEVHOOK_Update
* VC_DEVHOOK_Delete
