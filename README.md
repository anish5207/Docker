# Docker
This repository is made up for docker project. 

# Introduction:

This repository contains a complete setup for wordpress with mysql server inside the docker container.
WordPress is an online, open source website creation tool written in PHP. But in non-geek speak, it’s probably the easiest and most powerful blogging and website content management system 

# What is the need of docker ??

   -> When normally we do this it takes a lots of time to set up the environment for these servers , for installation           ,configuration & many more!!
   -> So, you can launch whole environment in just one click & can focuse on developing part except these things.
   -> you can also share your environment with your team mates by just cloning the container & by creating a image from        it.
# Software Requirenments:

-> In order to launch this set up you must have Docker & Docker compose installed on your computer having linux os.

# Steps:

 * Step 1:

    -> Clone this repository or download it in your computer .
    -> The directory structure should be like this:
        mycompository:-
           docker-compose.yml
           (and can be other files) 

  * Step 2:

     -> check the version of docker-compose by this command:
             docker-compose version
     -> Now you should be in lamp directory because in this directory we have our docker-compose.yml file .
        Now run this command :
             docker-compose up -d
     -> All the services will be run in background inside the docker containers.(because we used detach option in                 command).
   
   * Step 3:

      -> check ip address of your system by ifconfig command.
      -> It will give you many ip address but you have to concern about system's main network card.
      -> for Example : 192.168.40.130 this is your system's id.

    * Step 4:

      -> Go in your browser type this url in order to access web pages from web server: http://192.168.40.130:2000/ (It            will give you index file which is written in php.)
      
      -> Now for accessing phpmyadmin for managing mysql database write this url: http://192.168.40.130:7000/
      -> Note : here 2000 & 7000 are port no. that should be free in your system if they are not then you can change by            going inside the docker-compose.yml file




