# Update your Linda wallet to V3.2.0.0
## General Information
V3.2.0.0 has a few key changes in comparison to the previous (v3.1.0.1) wallet:
* Brand new interface (coded from scratch) for Windows, Mac and Linux (non-cli)
* First step in changing from the old (full block) to the new (head-first) syncing method
* More info: see v3.2.0.0 release notes

## Required steps to perform:
1. Open your wallet and make a backup BEFORE you continue with anything
2. Close your wallet when the backup is successful
3. Delete ALL Linda-QT files you have downloaded in the past, you don't need them anymore
4. Prepare your backend files for the new wallet (see in-depth below)
5. Install Altitude on your PC
6. Let it sync from scratch or use a bootstrap
7. Enjoy the new wallet!

## In-depth
1. Open your v3.1.0.1 (or older) wallet and go to `File` and click on `Backup Wallet...`.
Save this file on a secure location.
2. Close your wallet
3. Delete all Linda-QT files and/or shortcuts to these wallets, the new wallet lock all masternode inputs so you can stake in the same wallet.
Note: You can't run multiple Altitude instance on the same computer
4. Delete all files EXCEPT the `wallet.dat` file from the backend folder. __IF__ you have a `masternode.conf` there, don't delete it.
* Windows: Navigate to `C:/Users/YOURUSERNAME/Appdata/Roaming/Linda` or open your windows file explorer and type `%appdata%` and hit enter.
* Mac: Navigate to `~/Library/Application Support/Linda`. This is a hidden library. To enable it: Open Finder, click Go on the menu up top near the Apple logo in the corner. Hold down option on keyboard and you'll see library pop up under Go menu. That's the hidden library

Delete the files as explained above.

5. Download the Altitude installation file and perform the installation process
6. The v3.1.0.1 wallet needed around 36 hours for a sync from scratch, the new v3.2.0.0 will sync from scratch in a few (~6) hours. We did create a [v3.2.0.0 bootstrap](https://drive.google.com/open?id=1vJr59oEIKlPWUMo8Uzf87HOPKPETdOcj) if anyone wishes to use it.

Bootstrap steps:
* Close Altitude wallet
* Download the Bootstrap
* Unzip the bootstrap
* Replace the files in your application folder (see step 3 for the folder location) with the files from the bootstrap.
* Once done, open the Altitude wallet again. It will reindex all transactions.
7. Enjoy the new wallet!

## FAQ
### I have a question/problem
Join us on [Discord](https://discord.gg/SHNjQBv)!

### Can I update from an older version (v3.1.0.0 or earlier) directly to the new wallet?
Absolutely! You can follow the exact same steps as explained earlier.

Note: If you were staking on a side fork (example: if you was still using the v2 wallet), all transactions since the hard fork block will not appear!

### Multi-language Wallet
The new wallet is provided in multiple languages, these were automatically translated.

Language contributions are possible thru our [GitHub Altitude repo](https://github.com/TheLindaProjectInc/Altitude).
