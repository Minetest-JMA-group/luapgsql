A Lua Binding for PostgreSQL

Copyright (C) Micro Systems Marc Balmer.
You can reach the author at marc@msys.ch

Makefile is for BSD systems
GNUmakefile is for Linux systems

See https://lua.msys.ch/lua-module-reference.html#pgsql for full documentation.

Building for LuaJIT:
`make -f GNUmakefile LUA_VERSION=5.1 CFLAGS="-O3 -Wall -fPIC -I/usr/include/postgresql $(pkg-config --cflags luajit)" LDADD="-lpq $(pkg-config --libs luajit)"`
