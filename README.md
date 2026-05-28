# Nexus Android Manifest #

### Initialize Nexus ###

**Initialize full repository (useful for developers)**
```
repo init -u https://github.com/paranoid-nexus/android_manifest -b 15
```

**If you want to save space, use this instead**
```
repo init -u https://github.com/paranoid-nexus/android_manifest -b 15 --depth 1
```

### Sync Sauce ###
```
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags --optimized-fetch
```

### Build ROM ###
```
. build/envsetup.sh

brunch device
```

## Now Build and Enjoy! ##
