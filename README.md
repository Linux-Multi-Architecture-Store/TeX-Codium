# TeX-Codium
### Introduction
This is a TeX editor built with electron (maybe). 

As I previrously was a macOS user, I often use TexPad to write tex files. The _real-time compile_ function really impressed me. However, it does not provides Windows and Linux version, and it is expensive. This project intends to solve these problems, and I wish someone wants to support me!

### Development
You'll need the following tools:

 - Git
 - Node.JS, **x64**, version `>=16.14.x and <17`
 - Yarn, follow the installation guide
 - Python (required for node-gyp; check the node-gyp readme for the currently supported Python versions)
   - Note: Python will be automatically installed for Windows users through installing windows-build-tools npm module (see below)
 - A C/C++ compiler tool chain for your    platform:
   - Windows 10/11
     - Install the Windows Build Tools:
        - if you install Node on your system using the Node installer from the Node.JS page then ensure that you have installed the 'Tools for Native Modules'. Everything should work out of the box then.
        - if you use a node version manager like nvm or nvs then follow these steps:
          - Install the current version of Python using the Microsoft Store Package.
          - Install the Visual C++ Build Environment by either installing the Visual Studio Build Tools or the Visual Studio Community Edition. The minimum workload to install is 'Desktop Development with C++'.
          - open a command prompt and run npm config set msvs_version 2019
     - Warning: Make sure your profile path only contains ASCII letters, e.g. John, otherwise, it can lead to node-gyp usage problems (nodejs/node-gyp/issues#297)
     - Note: Building and debugging via the Windows subsystem for Linux (WSL) is currently not supported.
    - Windows WSL2: https://github.com/microsoft/vscode/wiki/Selfhosting-on-Windows-WSL
    - macOS
      - Xcode and the Command Line Tools, which will install gcc and the related toolchain containing make
        - Run `xcode-select --install` to install the Command Line Tools
    - Linux
      - On Debian-based Linux: `sudo apt-get install build-essential g++ libx11-dev libxkbfile-dev libsecret-1-dev python-is-python3`
      - On Red Hat-based Linux: `sudo yum groupinstall "Development Tools" && sudo yum install libX11-devel.x86_64 libxkbfile-devel.x86_64 libsecret-devel # or .i686.`
      - Others:
        - `make`
        - `pkg-config`
        - `GCC or another compile toolchain`
        - Dependencies:
          - Building deb and rpm packages requires `fakeroot` and `rpm`; run: `sudo apt-get install fakeroot rpm`