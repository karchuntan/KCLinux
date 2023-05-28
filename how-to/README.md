# How to?

## Run sudo command without a password

1. Open `/etc/sudoers` with `visudo` editor, as if straight away edit `/etc/sudoers` file with text editor, it won't validate the syntax
<<<<<<< Updated upstream
    ```bash
    sudo visudo
    ```
2. Append this line `username   ALL=(ALL:ALL) NOPASSWD:ALL` at the end of the `/etc/sudoers` file
    ```bash
    # User privilege specification
    root    ALL=(ALL:ALL) ALL
=======
 ```bash
 sudo visudo
 ```
2. Append this line `username   ALL=(ALL:ALL) NOPASSWD:ALL` at the end of the `/etc/sudoers` file
 ```bash
 # User privilege specification
 root    ALL=(ALL:ALL) ALL
>>>>>>> Stashed changes

    # Members of the admin group may gain root privileges
    %admin ALL=(ALL) ALL

    # Allow members of group sudo to execute any command
    %sudo   ALL=(ALL:ALL) ALL

    # See sudoers(5) for more information on "@include" directives:

<<<<<<< Updated upstream
    @includedir /etc/sudoers.d
    kc      ALL=(ALL:ALL) NOPASSWD:ALL
    ```
1. Open a new terminal window and test the command with **root** privileges
    ```bash
    sudo apt-get update
    ```
=======
 @includedir /etc/sudoers.d
 kc      ALL=(ALL:ALL) NOPASSWD:ALL
 ```
3. Open a new terminal window and test the command with **root** privileges
 ```bash
 sudo apt-get update
 ```
 
>>>>>>> Stashed changes
