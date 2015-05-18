This binary is the only one I've found to work with the NanoBeam (NBE)

After installing you will get a bug with LuCI http://dev.qmp.cat/issues/356

You just need to comment out the four lines (25, 51, 52, 53) that reference luci.fs in qmp.lua

Here is the [file with fixes](http://dev.qmp.cat/projects/qmp/repository/revisions/8526aa5d985ab2699fc55bc071fa98323dd81963/entry/packages/qmp-system/files/usr/lib/lua/luci/controller/qmp.lua). It is also inside this folder.

