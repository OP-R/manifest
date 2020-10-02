# OP-R #

### Sync ###

```bash

# Initialize local repository
repo init -u git://github.com/OP-R/manifest.git -b r-test

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch aosp_$device-userdebug

# Build the code
$ mka bacon -jX
```
