# Minecraft
Easily setup a vanilla minecraft from the command line!

## Usage
To get a 1.16.1 vanilla server running on the local machine at the standard port 25565 without any fuss, just run the script:
`./ezmc`

Ezmz will start the server by default, in a screen called 'Minecraft'. To exit the screen, hold CTRL and press A, then D.
You can resume the screen using `screen -r Minecraft`

Ezmc also allows you to specify the directory in which to install the server, the version, and the arguments with which
to run the server:
`./ezmc --install-path /path/to/mydir/ --version 1.16.3 --args "-Xms1024M -Xmx1024M nogui"`

Additionally, ezmc also allows for easy setup of a remote machine using SSH (an SSH key must be provided):
`./ezmc --remote --hostname example@example.com --key MyKey.pem`
