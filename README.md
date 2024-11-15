# android-studio-box
Container for Android Studio installation and runtime dependencies on Linux. Intended for atomic desktops.

This project aims to provide a ready-to-go container with all of the needed dependencies to install and run Android Studio on Linux. Primarily intended for users of image-based systems such as Fedora Atomic Desktops and Universal Blue images, but it can be used on any Linux distro that distrobox is available on. There is issues with the Flatpak version of Android Studio on atomic-based distros. This project aims to ease those issues.

# Requirements
You will need Podman/Docker as well as distrobox.

You will also need the latest release of Android Studio from Android's website.

# Setup

Open a terminal, then run `chmod +x /path/to/setup.sh`.

Then, `/path/to/setup.sh /path/to/android-studo-version-linux.tar.gz --home `.

Android Studio seems to pollute your `/home`, so please specify a folder where the home folder of the container will live. By default this is `$HOME/Distrobox/Android-Studio`.
