Getting Started

To get started with BrokenRoms, you'll need to get familiar with Git and Repo.

To initialize your local repository using the AOSP/CAF based BrokenRoms source, use this command:

repo init -u git://github.com/BrokenROM/platform_manifest.git -b lp5.1

Sync up with this command:

repo sync -f -jX (-f being for force and replace the X in -jX with the number of cpus/threads your box contains (WARNING: Going too high can severely drag performance)

Initiate the build with:

. build/envsetup.sh

Prepare your device with:

lunch (pick your devices number from the list)

Then fire it off with:

time make broken -jX (x being the amount of cores/threads your build box contains...Adjust accordingly, but going too high for your box can cause complications..Be warned)
