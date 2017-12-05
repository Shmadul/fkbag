# fkbag
Fix K-Bag issue when porting SwitchBoards
Method 1 (Pre-Install Method): 
* Place fixkeybag in root of rfs dmg
* Place launchd.conf in /private/etc/
* Make sure to chmod fixkeybag
* ASR Imagescan the DMG again
* Compress to zip and rename to ipsw and restore

Method 2 (Post-Install Method):
* Once you get error 37
* Put device into dfu mode
* Use SSHRD
* Connect to device over ssh and run mount.shmadul
* Copy fixkeybag to /
* Make sure to chmod fixkeybag
* Copy launchd.conf to /private/etc/
