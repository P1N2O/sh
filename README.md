Repository Structure
/lib: The core utility library (OS detection, validation, UI helpers).
/change-hostname: A universal script to safely update your machine's network name.
/init: (Coming Soon) A bootstrap script for fresh server setups.

🛠️ Developer Philosophy
POSIX First: Scripts are written for /bin/sh. This ensures they run on minimal environments like Alpine Docker containers without needing to install bash.

OS Agnostic: We detect if you are on BSD (macOS) or GNU (Linux) and adjust commands (like sed or hostname) accordingly.

Safe Execution:

Use -fsSL with curl to prevent executing 404 pages.

Scripts include strict input validation.

sudo is called internally only where necessary.

⚠️ Security Warning
Always inspect scripts before running them. While these scripts are maintained by , it is a best practice to check the source code of any script you pipe from the internet

📄 License
MIT
