
![Logo](https://raw.githubusercontent.com/ino-software/hyp.access/9b230ac2ad0a280bc9d99c21210045a6ad455d52/resources/img/banner.png)


*hyp.access* is a closed-source tool designed to make application installation and elevation accessible and seamless to standard users in a managed Windows environment, where they would otherwise not have permission.



![GitHub release (release name instead of tag name)](https://img.shields.io/github/v/release/ino-software/hyp.access)


## How it works

The application is installed via a bootable USB stick. It can be installed even if the individual installing it does not have administrative permissions on the target computer. The installation process copies files, installs services, and makes other reversible modifications to the users system that allow *hyp.access* to function. It also creates a special local user account, which is what will be used to elevate and run applications. The tool does not grant special permissions to the target user's account, nor provide any other way to access Administrative permissions; it is all done securely through *hyp.access*.

Once installed, the application seamlessly integrates with the user's desktop environment, providing easy access to settings and information from the Quick Launch section in the taskbar, and allowing the user to run any .exe, .msi, or .hya file using *hyp.access* with a button on the right click menu.

When an application is run using *hyp.access*, the user is presented with a prompt, much like a UAC prompt, to confirm that the application will be elevated and run with *hyp.access*. If the user continues, the *hyp.access* service will communicate with an authentication server, confirming that the user account, the IP address the user is communicating from, and the application they are trying to run are allowed by the server. If these conditions are met and validated, the application will be run with elevated privileges under the special *hyp.access* user account on the target user's desktop.

Administrator/s of a *hyp.access Server* can manage which users, IP addresses, and applications will be authenticated to run through the use of blacklists and whitelists.
## Data usage
*hyp.access* does not collect any information on its users, but any time it needs to authenticate an action, or query information, it must disclose your username, domain, IP address, and (if any) applications you attempt to run using the service to the authentication server you have connected it to. All communications with a *hyp.access Server* are automatically logged and stored locally by the server's operator, but not by the service on your computer, nor by any other third-parties. 

**The management of the personal data detailed above is at the sole discretion of your authentication server's Administrator(s). If you are concerned with how your information may be handled by the administrators of an authentication server, contact them and inquire about their policies surrounding the management of personal data. Ino does not have any control or access over information delivered to *hyp.access Server*(s) it does not operate.**
