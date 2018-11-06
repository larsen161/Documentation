# Linda - Bootstrap
Bootstrapping is the process for speeding up the syncing of your wallet. Syncing is your wallet downloading all transactions from when it was made until now. You can bootstrap your wallet to give it the file instead of it downloading slowly (syncing).

## Before you start
Backup your wallet

## Download dynamic bootstrap
Navigate in your browser to [bit.ly/lindabootstrap](https://bit.ly/lindabootstrap)

On the right top corner select Download & Direct download

## Content in bootstrap file
The zip file should contain 3 files and 2 folders
- Files: 
peers.dat,
blk0001.dat,
autoBootstrap.cmd
- Folders: 
database,
txleveldb

## Applying the bootstrap to Windows
Extract all content from the zip file downloaded above

Make sure Linda wallet is closed

Navigate to C:/Users/YOURUSERNAME/Appdata/Roaming/Linda or open your windows file explorer and type %appdata% and hit enter. This will open your C:/Users/YOURUSERNAME/Appdata/Roaming folder and navigate to the Linda folder.

Please note if Appdata folder is not visible. You will need to show hidden files by clicking the view tab and clicking the hidden files box

Copy extracted files to the Linda folder and when prompted click replace or replace all

## Applying the bootstrap to Mac
Extract files downloaded from the zip file downloaded above

Make sure Linda wallet is closed

Click Go in top menu bar and select go to folder

Enter the following in prompt box: ~/Library/Application Support/Linda

It is a hidden library to open it: Open Finder, click Go on the menu up topnear the Apple logo in the corner. Hold down option on keyboard and you'll see library pop up under Go menu. It will show the hidden libraries

Copy extracted files, except the autoBootstrap.cmd, to the Linda folder and when prompted click replace or replace all

## Applying the bootstrap to Linux
Make sure Linda Server is stopped using command Lindad stop

Change directory to Linda using command cd ~/.Linda

Download bootstrap using command wget -O Lindabootstrap.zip http://bit.ly/lindaboostrap?dl=1

Unzip bootstrap to Linda folder using command unzip Lindabootstrap.zip

When prompted press A and then enter to replace all files in folder

Please note if you get an error at the unzip stage, then run the command apt install unzip and then repeat the unzip command above

Start server using command Lindad -daemon 

