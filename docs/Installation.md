# Installing the Mobile Chrome Apps tools

## Node.js

## git

Windows:
* Install [msysgit](http://code.google.com/p/msysgit/downloads/list?q=full+installer+official+git)
  * Default options for the installer work fine

OS X:
* Install Xcode to get git.

Linux:
* Use your distribution's package manager.

## Install node.js

* Version 0.10.0 or greater is required.

Windows:
* Available from [nodejs.org](http://nodejs.org)
* But we recommend installation via [nodist](https://github.com/marcelklehr/nodist)

OS X & Linux:
* Available from [nodejs.org](http://nodejs.org)
* But we recommend installation via [nvm](https://github.com/creationix/nvm)

        curl https://raw.github.com/creationix/nvm/master/install.sh | sh
        source ~/.bash_profile
        nvm install 0.10
        nvm alias default 0.10

## iOS Dependencies

* iOS development can only be done on OS X.
* Install [Xcode 5](https://developer.apple.com/xcode/).
* You must register as an iOS developer for testing on real devices and for submitting to the app store.  You can skip this if you only plan to use the iPhone/iPad simulators.

## Android Dependencies

* Install Java JDK: [http://www.oracle.com/technetwork/java/javase/downloads/index.html](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
* Install the [Android SDK and Developer Tools](http://developer.android.com/sdk/index.html), which comes bundled with Eclipse.
  * Add `sdk/tools` and `sdk/platform-tools` [to your PATH](https://www.google.com/search?q=how+to+add+sdktools+to+path) environment variable.
* Install [Apache Ant](http://ant.apache.org/)
  * Add `apache-ant-x.x.x/bin` [to your PATH](https://www.google.com/search?q=how+to+add+sdktools+to+path) environment variable.


## Clone This Repository

* Clone this repository.  Then run `./mca init` to have it auto-install its dependencies.

        git clone git://github.com/MobileChromeApps/mobile-chrome-apps.git
        cd mobile-chrome-apps
        # This next step may take over a minute
        ./mca init
        # Optional - add the mca command globally:
        npm link


* On Windows, remove the "./" prefix from the last line.
* The `npm link` step is optional, but will add `mca` command to a global PATH if you have npm (node package manager) set up correctly.

## Experiencing Hiccups?

Please reach out to us at [mobile-chrome-apps@googlegroups.com](mailto:mobile-chrome-apps@googlegroups.com).

## Completed Successfully?

Now read the [Getting Started guide](GettingStarted.md).
