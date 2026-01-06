# FAQ for installation

### Table of contents

- [Special character in path](#space-or-special-character-in-the-path)
- [One drive installation](#try-avoiding-installation-in-one-drive)
- [Not admin + Press any key](#not-an-admin-message--press-any-key)
- [Explicitly activating virtual enviornment](#explicitly-activating-virtual-environment-python)

#### Windows specific:

- [Terminal exits immediately](#windows-program-starts-and-exits-immediately-closing-command-line)
- [Clicking opens notepad](#windows-clicking-on-file-opens-notepad)

#### Mac specific

- [Shell problems](#mac-bash-shell)
- [Operation not permissible](#mac-operation-not-permissible)
- [Changing superuser password (last resort)](#mac-changing-superuser-password-only-last-resort)
- [Installation takes too long/Homebrew issue (esp tools specific)](#mac-homebrew-issue-esp-tools-specific)

---

#### Space or special character in the path
- Not permissible. Beware of One Drive etc. 
- Create folder in `C:\Users\<user>\`
- Run in a `Public` user `C:\Users\Public`

#### Try avoiding installation in One Drive
- See the previous issue. 
- Documents and Desktop are typically a part of One Drive.

#### Not an admin message + Press any key
- Open terminal as administrator (right click on the icon).

#### Explicitly activating virtual environment (python)
- In case virtual environment is somehow not automatically detected/recognized
- `source db1/venv/bin/activate`

#### [Windows] Program starts and exits immediately closing command line
- You are running .ps1 file. Run .bat file instead.

#### [Windows] Clicking on file opens notepad
- Make sure you are opening .bat file. 

#### [Mac] Bash shell
- Command should be run as a `bash ./db1_installation.sh`.

#### [Mac] Operation not permissible 
- Downloaded files on mac may be flagged with com.apple.quarantine tag. 
- Remove it recursively: `xattr -dr com.apple.quarantine .` (remember space dot at the end!)

#### [Mac] Changing superuser password (only last resort)
- Might need to change superuser password.
  - Run `sudo passwd root` and follow the instructions.

#### [Mac] Homebrew issue (esp tools specific)
- Homebrew might take too long (more than 10 minutes).
- Happens when installation was previously interrupted.
- Install esp tools manually `python -m pip install esptool`
- Verify installation: `python -m esptool version`

