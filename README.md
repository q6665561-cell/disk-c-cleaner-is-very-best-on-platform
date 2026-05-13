# disk-c-cleaner-is-very-best-on-platform
Version 1.0 | Author: System Administrator | Date: 2026-05-13
Target OS: Windows 10 (Build 19045.7291) & Windows 11 (Build 26100.8457)

⚠️ Disclaimer
The author provides no warranties, either expressed or implied. This script is provided "as is" for system maintenance purposes. By executing this script, you acknowledge and agree that:

The script will perform a deep clean of drive C, removing all non-system files.

All user data (documents, downloads, desktop files), browser caches, browsing history, cookies, and Recycle Bin contents will be permanently deleted.

Installed programs and games will NOT be removed.

If your Windows version does not exactly match Windows 10 Build 19045.7291 or Windows 11 Build 26100.8457, the script may behave unpredictably and could potentially damage your operating system.

The author assumes no liability for any data loss, system instability, or other damages that may occur as a result of using this script.

It is your sole responsibility to back up all important data before proceeding.

📜 Script Description
This professional Python script is designed for a comprehensive, automated cleanup of the C: drive on Windows 10 and 11. It performs the following actions:

Clears User & System Junk:

User Temp files (%TEMP%).

System Temp files (C:\Windows\Temp).

Windows Update cache.

Windows Delivery Optimization files.

Empties Recycle Bin: Permanently deletes all files for all users using the Windows API.

Deep Cleans Browser Data (Chrome, Edge, Firefox):

Clears browser caches, cookies, history, and local storage for all user profiles found on the system.

Performs System Cleanup:

Runs the built-in cleanmgr (Disk Cleanup) tool silently for all available options.

Runs DISM to clean up the WinSxS component store.

Handles Missing Browser Scenario:

Checks if any major browser (Chrome, Firefox, Edge) is installed.

If no browser is found, it automatically downloads the latest Google Chrome offline installer and places it on the Public Desktop (C:\Users\Public\Desktop) with a clear message, ensuring the user can easily get online.

⚙️ System Requirements
Operating System: Windows 10 (Build 19045.7291) or Windows 11 (Build 26100.8457).

Privileges: The script MUST be run as Administrator. The user account running the script also needs a valid, active user profile.

Python: Python 3.6+ installed. No external libraries are required.
📝 How to Use
Save the script: Copy the code above into a new text file and save it as deep_cleanup.py.

Run as Administrator: Right-click on your cmd.exe or PowerShell shortcut and select "Run as Administrator". Navigate to the folder where you saved the script.

Execute: Run the script using python deep_cleanup.py.

Monitor: The script will generate a log file (deep_cleanup.log) in the same directory detailing every action it takes.

Restart: When finished, restart your computer for the best results. If a Chrome installer was needed, you'll find it on the Public Desktop along with a text file with instructions.
