# FAQ for installation

### Table of contents

- [Special character in path](#space-or-special-character-in-the-path)
- [One drive installation](#try-avoiding-installation-in-one-drive)
- [Not admin + Press any key](#not-an-admin-message--press-any-key)

#### Windows specific:

- [Terminal exits immediately](#windows-program-starts-and-exits-immediately-closing-command-line)
- [Clicking opens notepad](#windows-clicking-on-file-opens-notepad)

#### Mac specific

- [Shell problems](#mac-bash-shell)
- [Permission denied](#mac-permission-denied)

---

#### Space or special character in the path
- Not permissible. Beware of One Drive etc. 
- Create folder in `C:\Users\<user>\`
- Run in a `Public` user `C:\Users\Public`

#### Try avoiding installation in One Drive
- See the previous issue. 
- Documents and Desktop are typically part of One Drive.

#### Not an admin message + Press any key
- Open terminal as administrator (right click on the icon).

#### [Windows] Program starts and exits immediately closing command line
- You are running .ps1 file. Run .bat file instead.

#### [Windows] Clicking on file opens notepad
- Make sure you are opening .bat file. 

#### [Mac] Bash shell
- Command should be run as a `bash ./db1_installation.sh`.

#### [Mac] Permission denied
- Run `chmod +x ./db1_installation.sh`
- Might need to change superuser password.
  - Run `sudo passwd root` and follow the instructions.   