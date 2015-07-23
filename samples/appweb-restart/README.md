Appweb Restart
===

This sample allows to restart appweb servers 

Requirements
---
* [Appweb](https://embedthis.com/appweb/download.html)
* [MakeMe Build Tool](https://embedthis.com/e/download.html)

To run:
---
    sudo me run

The server listens on port 8080. Browse to:

     http://localhost:8080/
     http://localhost:8080/test.esp

Alternatively, run appweb to use the appweb.conf file.

    sudo appweb

Notes:
---
So that the Compiler is not required inside the jail, the ESP pages are pre-compiled before running Appweb.
Appweb is configured to load modules before changing the root directory via the "Chroot" directive in appweb.conf.

Code:
---
* [server.c](server.c) - Main program
* [appweb.conf](appweb.conf) - Appweb server configuration file
* [index.html](index.html) - Web page to serve
* [start.me](start.me) - MakeMe build instructions

Documentation:
---
* [Appweb Documentation](https://embedthis.com/appweb/doc/index.html)
* [Chroot Directive](https://embedthis.com/appweb/doc/users/dir/server.html#chroot)
* [Security Considerations](https://embedthis.com/appweb/doc/users/security.html)

See Also:
---
* [typical-server - Fully featured server and embedding API](../typical-server/README.md)