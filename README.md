# android-tools-AppImage
Unofficial AppImage of Android Platform Tools (adb, fastboot, etc), uses the official [binaries](https://developer.android.com/tools/releases/platform-tools) and turns them into an AppImage.

**This AppImage bundles everything and should work on any linux distro, even on musl based ones.**

You can also run the android-tools-appimage.sh script in your machine to make the AppImage.

If you are missing android udev rules you can usually get them from your distro repos or use the flag `--getudev` with the AppImage to install them. 

It is possible that this appimage may fail to work with appimagelauncher, since appimagelauncher is pretty much dead I recommend this alternative: https://github.com/ivan-hc/AM

You can also use [Soar](https://github.com/pkgforge/soar) to add this package as a [Nest](https://docs.pkgforge.dev/repositories/nests)
```bash
soar nest add "https://github.com/pkgforge-dev/android-tools-AppImage"
```

This appimage works without `fuse2` as it can use `fuse3` instead.
