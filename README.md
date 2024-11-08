# aosp_manifest
### Sync ###
```bash
        repo init -u https://github.com/Evilmove/aosp_manifest.git -b main --git-lfs
        repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###
```bash
	. build/envsetup.sh
        lunch aosp_<device code name>-ap3a-<build type>
         make bacon
