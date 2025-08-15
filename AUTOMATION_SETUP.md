# Setting up Automatic Sorting at OS Level

## Using launchd (macOS)

1. Create a plist file:

```bash
nano ~/Library/LaunchAgents/com.<your_username>.filesorter.plist


<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC ... >
<plist version="1.0">
<dict>
    <key>Label</key>
    <string>com.username.filesorter</string>
    <key>ProgramArguments</key>
    <array>
        <string>/usr/bin/python3</string>
        <string>/path/to/file_sorter.py</string>
    </array>
    <key>StartCalendarInterval</key>
    <dict>
        <key>Hour</key>
        <integer>9</integer>
        <key>Minute</key>
        <integer>0</integer>
    </dict>
    <key>RunAtLoad</key>
    <true/>
</dict>
</plist>


launchctl load ~/Library/LaunchAgents/com.<your_username>.filesorter.plist