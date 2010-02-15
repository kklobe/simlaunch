Simulator Launcher

== Introduction ==

Simulator Launcher builds custom executables to automatically launch an
embedded iPhone Simulator application using the correct iPhone SDK.

To use, drag any iPhone Simulator binary onto the "Simulator Builder" application. This will create
a new Mac OS X application that may be used to launch your own application from within Mac OSX. The
new application's icon and name will be derived from your iPhone Simulator application.

The launcher will:
- Detect all installed iPhone SDKs (such as the beta iPad SDK) using Spotlight,
  even if they're in non-standard locations
- Automatically select the best available SDK for your application.
- Install and launch your application in the appropriate Simulator.
- Works with both iPhone and iPad simulator binaries.

== Building ==

The project should build and run on Mac OS X 10.5 and 10.6. To build, run the disk image target:
    xcodebuild -configuration Release -target "Disk Image"

Building requires the PLBlocks 1.1-beta2 SDK to support blocks on 10.5:
    http://code.google.com/p/plblocks/

Binary releases of Simulator Launcher are also available from:
    http://github.com/landonf/simlaunch/downloads


== Authors ==

- Landon Fuller
- Erica Sadun