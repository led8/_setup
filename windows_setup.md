# Setup your machine!
___

Welcome to this setup where we are going to install the tools required to make your machine a true developer environment 💪. The following instructions will help you to get ready for The Ubisoft Legal Dev fullstack bootcamp:

- Install a code editor, where you will spend your days and nights
- Install a package manager
- Pimp your Terminal
- Setup git and GitHub
- Install Ruby


### Prerequisites
___

Before we start, it is important you meet the following prerequisites to ensure the smooth running of the setup. Take your time to read through everything and do not hesitate to ask for help if you feel stuck. Ready? Let's go 😎

##### Latest version of Windows
For this setup, you need to be using the latest version of Windows.

This means that you need to be on Windows 10, with all the latest updates installed.

You can check your software version by clicking on **Start>Settings>System>About**. Look where it says **Edition**. If you see something that starts with "Windows 10..." you're good to go 💪.

Not the case? Don't panic 😱 You can always install Windows 10 from [Microsoft](https://www.microsoft.com/en-gb/windows/get-windows-10) (it should take roughly an hour to install but this is dependent on your computer). Click on **Check for Updates**, then follow the instructions on the screen. Come back to this setup when Windows 10 is installed.

Once you're sure that you're using Windows 10, you will need to check that your computer has all the latest updates. For this click on **Start>Settings>Updates & Security>Windows Update**, then click on **Check updates**. If you have updates available please install them and repeat the process until it says that you are up to date ⭐.

##### The Insider program
For the best development tools we need to be part of the **Windows Insider** program which gives access to pre-release versions of various tools.

Go to **Start → Settings → Updates & Security → Insider Program**

Click on **Get Started**. It will ask you to **Link an account**; follow the instructions on screen. You will be asked to choose your Insider parameters, choose the second setting, the **fast** one ⚡. Then confirm and restart your computer when you are asked to do so.

After your computer has restarted you can double-check that you are now part of the Insider program by clicking on **Start → Settings → Updates & Security → Insider Program.** You should then be prompted with the Insider parameter that you chose earlier, i.e. fast.

By joining the Insider program you have unlocked more content and updates — which we also need to install. Go to **Start → Settings → Updates & Security → Windows Update,** you should see new updates available. ⚠️ These updates can take a rather long time of more than 30 minutes, so make sure your computer has enough battery left, and that you won't have to close it during the installation ⚠️

Start the update and go grab a coffee ☕ or tea 🍵.

After your computer has restarted, go to **Start → Settings → System → About**. This time check the **Version**, if it says at least 2004, you are good to go 😎.

##### Virtualization
We need to ensure that the Virtualization options are enabled in the BIOS of your computer.

For many computers, this is already the case. Let's check:

- Press Ctrl + Alt + Del.
- Select Task Manager.
- Click on the Performance tab.
- Click on CPU.
- The status will be listed under the graph and will say "Virtualization: Enabled" if this tool is enabled.


### GitHub account
___
Have you signed up to GitHub? If not, [do it right away](https://github.com/).

👉 [Upload a picture](https://github.com/settings/profile) and put your name correctly on your GitHub account. This is important as we'll use an internal dashboard with your avatars. Please do this now, before you continue with this guide.

### Windows Subsystem for Linux
___

WSL is the development environment we are using to run Ubuntu. You can learn more about WSL [here](https://docs.microsoft.com/en-us/windows/wsl/faq).

Click on **Start** and type **powershell**. Right click on **Windows Powershell**, then on **Run as administrator**. A blue terminal window will appear. Copy the following commands, paste them into the terminal windows by right-clicking into it, and run them by pressing Enter:

(If you are asked to restart your computer, type **n** and **enter** to prevent your computer from restarting at that moment).

```
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```

```
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```

````
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
````

**When all three commands ran without any errors, restart your computer**.

Once your computer has restarted, click on **Start** and type **Microsoft Store**. Launch it. In the search bar, type **Ubuntu**. Click on the result that says **Ubuntu plainly**, not **Ubuntu 18.04 LTS**. Then, click on **Install**.

⚠️ There is no progress bar for this installation. When it is done you will be asked, in the bottom right corner, to launch it.

The first time you open WSL - you will be asked to choose a username ⚠️. Your username should **be one word, lowercase** with **no special characters** ⚠️, for example: `legaldevbootcamp.`

It will then ask you for a new password. When you type your password, ⚠️ it will not appear on the screen ⚠️ – and there will be no familiar typing indicator even though your keystrokes are being registered. This is a security feature to mask not only your password as a whole but also its length!

You will have to retype your password, and then the installation should be complete.

You can close the terminal now that WSL is installed on your computer.
