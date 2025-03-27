# SPY-WARE

---

**SPYWARE**

**REVERSE SHELL EXECUTION**

A reverse shell will be executed on a machine within the same network, and from there we run a script to capture screenshots of that machine and save them in a folder.

Using NETCAT the attacker connects to the victim's machine.

Then, on the attacker's machine, we make it listen on port 1234.

We execute the following command, which is used to initiate a bash shell while running within the script command. In this case, however, it redirects the output to /dev/null so that it is not saved to a file.

We create a .sh script that takes screenshots in .xwd format (as it is a tool included by default in Kali), and send the screenshots via port 4321.

Next, we grant execution permissions to the script, execute it, and stop it after a while.

Here, we listen on the script's port (4321) and redirect the output to a .xwd file in the same folder.

We can see that a .xwd file has been created.

Finally we use an online converter to turn the .xwd file into a .jpg file:  
[https://convertio.co/xwd-jpg/](https://convertio.co/xwd-jpg/)

We upload the file, convert it, and download it. Upon opening it, this is what we get.

Everything worked perfectly—this process is used to spy on a machine and steal its information.

---


