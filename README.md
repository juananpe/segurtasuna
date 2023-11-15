# Dockerized pentesterlab for SQLi

## Dependencies:

* Windows:
  - Install Docker Desktop: https://docs.docker.com/desktop/install/windows-install/
  - Open a PowerShell terminal
* Ubuntu:
  - Install docker: https://docs.docker.com/engine/install/ubuntu/#installation-methods
  - Add your user to docker group.   **Run this command in your favourite shell and then completely log out of your account and log back in** (or exit your SSH session and reconnect, **if in doubt, reboot the computer** you are trying to run docker on!): 
           ``sudo usermod -a -G docker $USER``
  - Try to list running containers: (you should get an empty list, without errors)
  ``docker ps``
  - Install docker compose
  ``sudo apt install docker-compose``


* macOS:
  - Install docker desktop: https://hub.docker.com/editions/community/docker-ce-desktop-mac/

## How to use
* Clone the repo:
``git clone https://github.com/juananpe/segurtasuna.git && cd segurtasuna``
* Open a new terminal and run:

``chmod a+w www/admin/uploads/``

``docker-compose up``

If you want to stop the container, open a new terminal and run:
``docker-compose down``

## Screenshot

![Running SQLi Lab](https://ikasten.io/images/sqli_pentestlab.png)

## Credits:
This lab is a Dockerized version of https://pentesterlab.com/exercises/from_sqli_to_shell for educational purposes only
