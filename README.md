bash.origin.nw
==============

A plugin for [Bash.Origin](https://github.com/bash-origin/bash.origin) that installs [NW.js](http://nwjs.io/).


Usage
-----

	#!/bin/bash
	# Source https://github.com/cadorn/bash.origin
	. "$HOME/.bash.origin"
	function init {
		eval BO_SELF_BASH_SOURCE="$BO_READ_SELF_BASH_SOURCE"
		BO_deriveSelfDir ___TMP___ "$BO_SELF_BASH_SOURCE"
		local __BO_DIR__="$___TMP___"


		BO_callPlugin "bash.origin.nw" run "$__BO_DIR__/demo-app"
	}
	init


Test
----

	./test


API
---

### `run ...`

Calls `nw` passing along all arguments.


License
=======

Original Author: [Christoph Dorn](http://christophdorn.com)

[UNLICENSE](http://unlicense.org/)

