# speed test

## install 
https://www.speedtest.net/apps/cli

```sh
brew tap teamookla/speedtest
brew update
brew install speedtest --force
```

## use

[Introducing Speedtest® CLI](https://www.speedtest.net/insights/blog/introducing-speedtest-cli/)

```sh
$ speedtest

   Speedtest by Ookla

     Server: xxx-xxx - xxxx xxxx (id = 12635)
        ISP: VNPT
    Latency:     4.26 ms   (0.64 ms jitter)
   Download:    67.36 Mbps (data used: 80.5 MB)
     Upload:    69.35 Mbps (data used: 125.9 MB)
Packet Loss:     0.0%
 Result URL: https://www.speedtest.net/result/c/xxxxxxxxxxxxxxxxxxxxxxxx
```


# update hosts file

```sh
sudo vi /private/etc/hosts
```


# How to Clear DNS Cache in macOS Mojave

```sh
sudo killall -HUP mDNSResponder; sleep 2;
```

# List All Drives

```sh

$ df -H
Filesystem      Size   Used  Avail Capacity iused      ifree %iused  Mounted on
/dev/disk1s1    500G    11G    52G    18%  487880 4881965000    0%   /
devfs           197k   197k     0B   100%     667          0  100%   /dev
/dev/disk1s2    500G   435G    52G    90% 4837640 4877615240    0%   /System/Volumes/Data
/dev/disk1s5    500G   1.1G    52G     3%       1 4882452879    0%   /private/var/vm
map auto_home     0B     0B     0B   100%       0          0  100%   /System/Volumes/Data/home
/dev/disk2s1    2.1T    12M   2.1T     1%      89   15999406    0%   /Volumes/Untitled

$ diskutil list
/dev/disk0 (internal, physical):
   #:                       TYPE NAME                    SIZE       IDENTIFIER
   0:      GUID_partition_scheme                        *500.3 GB   disk0
   1:                        EFI EFI                     314.6 MB   disk0s1
   2:                 Apple_APFS Container disk1         500.0 GB   disk0s2

/dev/disk1 (synthesized):
   #:                       TYPE NAME                    SIZE       IDENTIFIER
   0:      APFS Container Scheme -                      +500.0 GB   disk1
                                 Physical Store disk0s2
   1:                APFS Volume Macintosh HD            11.0 GB    disk1s1
   2:                APFS Volume Macintosh HD - Data     435.1 GB   disk1s2
   3:                APFS Volume Preboot                 81.8 MB    disk1s3
   4:                APFS Volume Recovery                535.9 MB   disk1s4
   5:                APFS Volume VM                      1.1 GB     disk1s5

/dev/disk2 (external, physical):
   #:                       TYPE NAME                    SIZE       IDENTIFIER
   0:     FDisk_partition_scheme                        *2.1 TB     disk2
   1:               Windows_NTFS                         2.1 TB     disk2s1
```

# move to external drive

```sh
$ cd /Volumes/Untitled
```



# Move your content to a new Mac

[Move your content to a new Mac - Apple Support](https://support.apple.com/en-us/HT204350)


Transferring data from an old Mac to a new one using Migration Assistant is a straightforward process. Here's a step-by-step guide on how to do it:

1. Start by connecting both your old and new Macs to the same Wi-Fi network or connect them using an Ethernet cable.

2. On your new Mac, go to the "Applications" folder and open the "Utilities" folder. Then, launch "Migration Assistant."

3. In the Migration Assistant window that appears, select the option "From a Mac, Time Machine backup, or startup disk" and click "Continue."

4. On your old Mac, open "Migration Assistant" from the "Utilities" folder. If prompted, enter your administrator password.

5. In the Migration Assistant window on your old Mac, select the option "To another Mac" and click "Continue."

6. You will now see a security code displayed on both Macs. Make sure the code on your new Mac matches the one on your old Mac. If they match, click "Continue."

7. On your old Mac, you'll be asked to select the data you want to transfer to the new Mac. You can choose to transfer files, applications, user accounts, and other settings. Select the options you prefer and click "Continue."

8. The migration process will now begin, and the data from your old Mac will be transferred to the new one. This may take some time depending on the amount of data being transferred.

9. Once the migration is complete, you'll see a summary of what was transferred. Click "Quit" on both Macs to exit the Migration Assistant.

10. Finally, you can disconnect the old Mac from the network and continue using your new Mac with all the transferred data.

That's it! Your new Mac should now have all the data and settings from your old Mac thanks to the Migration Assistant.

# keyboard customizer

[Karabiner-Elements](https://karabiner-elements.pqrs.org/)



# How to prevent creation of .DS_Store files

```
defaults write com.apple.desktopservices DSDontWriteNetworkStores -bool TRUE

Killall Finder
```



