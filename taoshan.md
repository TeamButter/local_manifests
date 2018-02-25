## How to build
This doc contains instructions for building LineageOS 15.1 for taoshan.

### Requirements
* Android build environment set up. See https://source.android.com/setup/initializing for setting it up.
* Minimum of 8GB RAM.
* Lots of free storage.
* Basic knowledge of terminal commands.

### Downloading the source
* Initialize the repo in a directory of your choice. See https://github.com/LineageOS/android#getting-started to set up repo, but don't execute the `repo sync` command yet.
* Now get the device manifest:
```
cd .repo
git clone https://github.com/TeamButter/local_manifests -b lineage-15.1-taoshan
```
* Now repo sync:
```
cd ..
repo sync
```

### Build
* After repo sync is complete, start building with the command `source build/envsetup.sh && brunch taoshan`
