# What is this?

This is a work in progress branch that shows how to make Atom talk to Neovim.

# What's new?
I've update everything to work with the version in master of
[Neovim](http://github.com/neovim/neovim)

On the Atom side I've tested it with version 0.175 and 0.184 and seems to work
fine.

# How do you run this?

NVIM_LISTEN_ADDRESS=/path/to/listen/address /path/to/nvim -T abstract_ui

Then you will need to configure the value of CONNECT_TO in line 11 of
vim-state.coffee to /path/to/listen/address

# What do you want to do with this?

This project aims to:

* Bring real vim bindings to Atom.
* Give the abstract-ui neovim patch a work out and find issues using the
msgpack api.
* Eventually build an editor that I would find useful. At the current state it is
pre-alpha.

# See it in action

A new video of the integration in action, using the abstract-ui branch:

https://www.youtube.com/watch?v=yluIxQRjUCk

and this is an older video using the old redraw-events branch (from mid 2014):

http://www.youtube.com/watch?v=lH_zb7X6mZw

# Things TO DO

* Handle Atom-centric text editing actions, i.e., situations like the user
searching and replacing in Atom by hitting Cmd-F
* Make the client use less CPU. It currently uses a lot of CPU, this could be a
consequence of my limited CoffeeScript experience.

# Contributing

1. Find something that doesn't work (this step shouldn't be that hard, plenty
of things don't work yet)
2. Fix it. 
3. Send me a pull request.



