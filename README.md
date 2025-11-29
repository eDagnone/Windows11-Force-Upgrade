# Windows 11 Force Upgrade

Force an in-place update from Windows 10 to 11 on unsupported computers, keeping all documents, programs, and the Windows license.

This is intended to be used with an installer USB, and requires a USB stick (or other spare storage device) at least 8Gb in size. After this, you can either use the drive to update any computer you connect it to, or hand the drive off to someone so they can do it themselves.

## Making the USB Updater

1. Download the [Windows 11 ISO](https://www.microsoft.com/en-us/software-download/windows11) from Microsoft
2. Download [Rufus](https://github.com/pbatard/rufus/releases)
3. Use Rufus to write the Windows 11 image to the USB drive, and enable the following:
   - Remove Requirement for 4GB RAM, Secure Boot and TPM 2.0
   - Remove  requirement for anonline Microsoft account
   - Disable Data collection (Skip privacy questions)
4. Copy the files from this repository to the drive

## Using the USB Updater

1. Plug it in and open it
2. Double-click RUN_THIS.bat
3. Click through the standard Windows 11 upgrade tool to complete the upgrade

## Software Versions Tested

While the versions of your tools shouldn't matter (as long as they are up to date) - here are the versions of everything I used.

- Updated from: Windows 10 22H2 (final released version - no more updates available)
- Updated to: Windows 11 25H2
- Rufus Version: 4.11


## References

- [r/Windows11](https://www.reddit.com/r/Windows11/comments/1m8zkb6/windows_11_inplace_upgrade_on_unsupported/): Outlines process and registry kesy
- [asheroto's gist](https://gist.github.com/asheroto/5087d2a38b311b0c92be2a4f23f92d3e): Sets registry keys
