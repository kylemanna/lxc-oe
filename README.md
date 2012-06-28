lxc-oe
======

Author: Kyle Manna <kyle@kylemanna.com>

Linux Container (LXC) templates for repeatable Open Embedded builds by providing a sane build environment.

The intended procedure for building with OE:
1. Download this template to /usr/lib/lxc/templates
2. Create a LXC with lxc-create -t ubuntu-oe -n build0
3. Start the LXC with lxc-start -n build0
4. Determine the IP address of the LXC
5. SSH in to the LXC and proceed with a OE based build
6. Copy the resulting rootfs binary out


Roadmap:
* Get initial build support reliable
* Add support for performing a basic OE build and using it as a "stage 1" build and will be followed by an ephermeral "stage 2" that then can update the stage 1 build and complete the build followed by copying the resulting rootfs.

Feel free to submit patches via pull requests or send them to me.
