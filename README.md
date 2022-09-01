# tequilaOS

### Sync ###

```bash
# Initialize local repository
repo init -u https://github.com/tequilaOS/platform_manifest -b tobacco

# Sync
repo sync -c --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune -j$(nproc --all)
```

### Build ###

```bash
# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch tequila_$device-userdebug

# Build the code
$ mka bacon -jX
```