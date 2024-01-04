# flipper-badusb-ps3hen
This repo automates the installation of PS3Hen on compatible Playstation 3 consoles using a Flipper Zero as a BadUSB device

Based off instructions by [ConsoleMods](https://consolemods.org/wiki/PS3:PS3HEN)

## What this script does

* Opens the browser
* Sets the browser to exit without confirmation
* Sets the homepage to about:blank
* Deletes cookies, search history, cache and authentication information
* Closes the browser and opens it again
* Navigates to the exploit website and selects the correct menu options
* When the script resumes, opens Remote Play, then closes it
* Opens the Install HEN app then kicks off the installation

## Usage

0. Read the script first and understand it so you know what it's doing, and make sure it's not doing anything suss. This applies to everything you run, BadUSB, Javascript snippets, bash / batch scripts, EVERYTHING
1. Copy PS3HEN.txt to the badusb folder on your Flipper Zero
2. Follow steps 1-4 on the ConsoleMods instructions
3. Move over to the Network category in XMB and make sure Internet Browser is highlighted, **but don't run it**!
4. On your Flipper Zero, go to BadUSB and run the PS3HEN script. Plug your Flipper Zero into the PS3, then run the script.
5. The script will begin doing its work. If you find that the script is too fast, adjust the `DEFAULTDELAY` towards the top of the script, as well as any other `DELAY`s as necessary
6. There is a point in the script where you must press a button to continue. This occurs when exploit begins (step 13 in the ConsoleMods page) because the process takes an unknown amount of time and may fail. If it fails, either stop the script and follow step 13 from the ConsoleMods page onwards, or just close out of the browser, highlight the Internet Browser and run the script again

## Troubleshooting

Please don't submit issues relating to the ConsoleMods page. I'm not here to diagnose issues with you installing PS3HEN on your Playstation 3. However, if this script fails (e.g. it presses a button too quickly or something), I'd prefer you submit a Pull Request instead of an issue.

But if the script fails at some point, just stop it, go back to the Internet Browser icon in the XMB then run the script again

## To do / wishlist

- [ ] Automate the installation of the PS3 update in a way that works across PS3 versions as some versions have slightly different menus?
- [ ] See if I can reboot the PS3 using the keyboard
- [ ] Install Irisman and / or other packages
