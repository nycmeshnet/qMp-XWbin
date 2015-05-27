This binary is the only one I've found to work with the NanoBeam NBE-M5-19

After flashing you will get this bug with LuCI- http://dev.qmp.cat/issues/342

You just need to comment out the four lines (25, 51, 52, 53) that reference luci.fs in qmp.lua

The file lives here-
/usr/lib/lua/luci/controller/qmp.lua

Here is the [file with fixes](http://dev.qmp.cat/projects/qmp/repository/revisions/8526aa5d985ab2699fc55bc071fa98323dd81963/entry/packages/qmp-system/files/usr/lib/lua/luci/controller/qmp.lua). It is also inside this folder.

Thanks to Roger at qMp for emailing me the binaries.



