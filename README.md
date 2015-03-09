1.Download the repo from GitHub. The repository contains the following structure as described below.
  a) README.md: This file contains a brief description about all the folders present inside the repository. 
  b) Build: Initially this is an empty folder. But after executing the 'makefile' in the 'src' folder, all the contents of the lab will be copied here.
  c) Scripts: This folder contains the following files-
      i) .netrc: It contains the machine name, username and password of GitHub user.
     ii) build.sh: Build Script runs the makefile and copies the build folder to localhost. The script is invoked by initialize script.  
    iii) dependencies.txt: It contains all the dependencies to run the lab.
     iv) initialize.sh: initialize script creates the initial environment for the required lab by installing the server side dependencies for the lab and invokes the build script.It mention all the server-side dependencies of the lab in dependencies.txt. We have the following shell scripts for different environments- initialize ubuntu.sh,initialize fedora.sh, initialize centos.sh, initialize windows.bat.
      v) labspec.json : It has the build requirements, lab description, runtime environments for the required lab.
  d) src: This folder contains all the sources of the particular lab. It also has a 'makefile' which will copy the lab source contents to the 'Build' folder.

2. Based on your OS, execute the "initialize-<OS>.sh" script. You need to have root permission for successfully updating the required softwares and installation of the files. 
   
