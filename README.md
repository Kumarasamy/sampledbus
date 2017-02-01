# sampledbus
c++ dbus application

Build command for Adaptor:
==========================
g++ -I/usr/local/include/dbus-c++-1/ adaptor.cpp -ldbus-c++-1 -o adaptor

Build command for Proxy:
========================
g++ -I/usr/local/include/dbus-c++-1/ adaptor.cpp -ldbus-c++-1 -o adaptor

Lib used:
=========
libdbus-c++-devel
dbusxx-xml2cpp

Code gen command:
================
dbusxx-xml2cpp service.xml - -proxy=proxy.hpp - -adaptor=adaptor.hpp

Reference:
http://blog.emilienkia.net/post/2012/11/07/Journey-into-the-world-of-DBus-for-C-(part-2)-attempt-around-libdbus-c
