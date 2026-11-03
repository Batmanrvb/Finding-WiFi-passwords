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

## Theory
This tool is a Python script that retrieves and displays the Wi-Fi network profiles and their associated passwords stored on a Windows system using the subprocess module to run Command Prompt commands. The principle used here is essentially using the subprocess module to interact with the Windows command line and execute specific commands.

**1. Importing the Subprocess Module:** Here, we start by importing the 'subprocess' module, which allows you to spawn new processes, connect to their input/output/error pipes, and obtain their return codes.

**2. Running Command:** The script uses 'subprocess.check_output' to run specific Windows command line commands. In this case, it's running the netsh wlan show profiles command to retrieve a list of Wi-Fi network profiles on the system.

**3. Parsing Output:** The output of the command is captured, decoded from bytes to a UTF-8 string, and then split into lines. The code extracts the Wi-Fi profile names (SSID names) by looking for lines containing "All User Profile" and then extracting the profile names.

**4. Iterating Through Profiles:** It then iterates through the list of profiles and, for each profile, uses subprocess.check_output again to run netsh wlan show profile <profile_name> key=clear to retrieve the key (password) for each Wi-Fi network profile.

**5. Parsing Passwords:** Similar to the previous step, the output is captured, decoded, split into lines, and the password (Key Content) for each profile is extracted.

**6. Printing Results:** The code attempts to print the profile name and its associated password in a formatted way using print. If a password is not found for a profile, it prints an empty string.

**7. User Input:** Finally, the input("") line is used to keep the command prompt window open so that the results are visible to the user before the window closes.

**In summary, this tool demonstrates the principle of using the subprocess module to interact with the Windows command line, run specific commands, capture their output, and then parse and display the relevant information, which, in this case, is the list of Wi-Fi profiles and their passwords.** 

