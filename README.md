iet-platform
==============

Install the `repo` utility:

$: mkdir ~/bin  
$: curl http://commondatastorage.googleapis.com/git-repo-downloads/repo > ~/bin/repo  
$: chmod a+x ~/bin/repo  

Download the BSP source:

$: PATH=${PATH}:~/bin  
$: mkdir iet-bsp  
$: cd iet-bsp  
$: repo init -u https://github.com/jmore-reachtech/iet-platform -b jethro  
$: repo sync  

Once this has completed, you will have all you need. To start a build:

$: DISTRO=reach MACHINE=g2c-4_3-inch source ./setup-environment build  
$: bitbake iet-image-qt4e 
(and grab a few coffees)  
