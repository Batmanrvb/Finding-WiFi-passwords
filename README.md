# Finding wifi passwords Using Python
You can use this Python script to find your wireless password. Two commands must be run on the terminal in order to find the wifi passwords for devices that are already connected, hence in this programme, a Python script is used to execute these two commands. 

Please take note that this Python script only displays WiFi passwords for WiFi networks that were initially joined to the machine. For the unknown wifi network and any other nearby wifi networks, this script won't be able to locate wifi passwords.

## Explanation

To find the wifi passwords we need to run two commands on the terminal so to run commands using python scripts we need to import the python subprocess module. subprocess module allows you to spawn a new process. 

The two below commands are used to check the wifi passwords: 
```
$ netsh wlan show profile

```

```
$ netsh wlan show profile PROFILE-NAME key=clear

```

**The first command locates the profiles of the WiFi networks that are currently connected, and the second command displays the WiFi network's password.**

