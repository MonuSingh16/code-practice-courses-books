### Install WSL 2 and Ubuntu, and get the Ubuntu shell up and running.

1. [ ] Make sure you're on Windows 10 or 11. If you are on an older version, please upgrade. Your life as a developer will not be fun if you're on an older version of Windows.
    - [ ] Run Windows Update
    - [ ] Click on the start menu and begin typing "Windows update". You should see a program called "Windows Update Settings", open that.
    - [ ] Click "check for updates", and if there are any updates, install them and restart your computer as instructed by the updater.
    - [ ] Open the Windows Command Prompt and install WSL
    - [ ] Click on the start menu and begin typing "cmd.exe". You should see a program called "Command Prompt", right-click on it and select "Run as administrator".
    - [ ] Type wsl --install in the prompt and press enter. (If that comes up as invalid, use wsl --install -d Ubuntu)

2. [ ] Restart your computer
    - [ ] Confirm wsl is installed by running wsl -l -v in Command Prompt.
    - [ ] Set up the Ubuntu distro. Ubuntu is a very popular distribution (or distro) of Linux, and it was installed automatically alongside WSL.

3. [ ] After restarting your computer in step 3, you should see an "Ubuntu" Window open automatically once you log back in. If you don't, search for the "Ubuntu" program in the start menu and launch it.

4. [ ] The Ubuntu window will prompt you to enter a username and password (which may not appear when typed). Make sure you remember these! These are the credentials for your Linux user. Later when you need to enter your password for certain commands, you'll need to re-enter this password. Note: by default Ubuntu only accepts usernames in lowercase.