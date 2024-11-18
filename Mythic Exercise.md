## Mythic C2 

### Installation

- First you will need to clone Mythic from Github. `git clone https://github.com/its-a-feature/Mythic`
- If you do not have Docker installed. You will need to install it. I recommend that you use the script provided(`./install-docker-kali.sh`); however, if you can't (or if it doesn't work) follow these steps:
    - `sudo apt install docker.io`
    - `sudo apt install docker-compose`
    - `sudo apt install docker-compose-plugin`
- Next you need to make the CLI binary. To do this, run `sudo make`
- You are going to want to start the Mythic C2 Framework. To do this, run the command `sudo ./mythic-cli start`
    - This is going to give you a C2 framework with no agents or listeners. Mythic has many of these (and you can even create your own)! We are going to use Apollo and Websockets. 
    - To intall both, run the following commands:
        - `sudo ./mythic-cli install github https://github.com/MythicAgents/Apollo.git`
        - `sudo ./mythic-cli install github https://github.com/MythicC2Profiles/websocket.git`
    -  These commands can be run when mythic is running

### Using Mythic

Mythic is a complex C2 Framework that and has many features. For this exercise we are going to focus on getting you up and running with the framework!