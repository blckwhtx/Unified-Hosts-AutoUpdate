# Unified Hosts AutoUpdate
AutoUpdate script for Unified Hosts.

This AutoUpdate project is maintained by ScriptTiger: https://github.com/ScriptTiger/DualServer

The Unified Hosts project is maintained by StevenBlack: https://github.com/StevenBlack/hosts

Wget is also a component to this project licensed separately in accordance with its attached documentation.

Further project contributors are noted with their contributions in the Unified Hosts data, both available online from Steven Black's project as well as in the data injected into the local hosts file by this script, as it is downloaded directly from Steven Black's most recently pre-generated Unified Hosts files.

Just extract the contents and run the Hosts_Update.cmd script. If you plan to always update your hosts file with the same blacklist preferences, you can change the "URL" variable at the top of the script with the URL of the blacklist you prefer to use. There is also an option to remove the Unified Hosts from your local hosts file.

Also, if you send your prefered URL to the script as a parameter, it will bypass all the prompts and automatically install/update the Unified Hosts in the local hosts file. This is useful for things like scheduling a task to update your Unified Hosts daily or weekly, etc. If you do decide to make a scheduled task, also remember the account issuing the task must still have administrative privileges to be able to write to the local hosts file.

Because no backup of your local hosts file is needed, entries in the Unified Hosts relating to the localhost and other loopback addresses have been removed to prevent possible conflict with preexisting entries. No backup is needed because this script implements the Unified Hosts within opening and closing tags to clearly segment it from the user's preexisting entries and allow the script to know what area of the file to overwrite during an update or remove during removal.