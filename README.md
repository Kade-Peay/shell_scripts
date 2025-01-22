# What is this and what is the point?
This is simply a collection (ever growing) of shell scripts that I have enjoyed having on my machines. These range from silly ones, like a dedicated fibonacci sequence right on the terminal, to more useful ones; like system info and updating a slew of Raspberry Pi's on my network.

# Are you a bash master? Does this contain all the answers?
Not even close. I am relatively new to bash scripting, and these are simple tools I have built specifically for my own use cases. But my hope is much smarter individuals will use these a baseline for much better scripts.

## Adding to path
Run this line to make it temporary or add this line to your '.bashrc' to make it permanent:

``` export PATH=$PATH:~/path/to/shellScripts ```

You may have to run:
``` source ~/path/to/shellScripts ```
or restart you terminal for it to take effect.


## Scripts and what they do
* fib
    * Enter 'fib {sum_num}' and get the sequence up to that number.
* ghost
    * Says "BOO!".
* git-init-repo
    * Does the entire First commit for you. Defaults to adding all files to being tracked and pushing from main branch.
    * It will ask for the origin at the start.
    * It will also check and make sure current directory is not already a git repository.
* organize
    * NOT WORKING CURRENTLY!
    * Meant to organize /Downloads folder by file extension.
    * I wrote a better version in Python 5 years ago, I've fallen off.
* system_info
    * Gives Hostname, OS, Kernel Version, Uptime, Disk Usage, and Memory Usage.
* update_servers
    * Updates a list of servers. The list is my set of Raspberry Pi servers.
    * For this to work you must use 'ssh-copy-id' so that you don't have to individually log into every server. Is this safe and secure? Not at all. But it's my house and I'm a bad boy.
