# treebuilder

For some reason you're here wondering if you can use this tool to visualize the internal structure of an index of yours.

It requires python3.6.*. You'll also have to install pageinspect (https://www.postgresql.org/docs/10/static/pageinspect.html) extension.

You can clone this and then run

`python setup.py develop`

The command line is then

`python inspector/command.py --host <host> --port <port> --db <your_db> --user <youruser> --index <index_name> --path <your_path>`

It will generate a wonderful html.<your path> is the path of the html file to be saved (e.g. home/user/test.hrml).

It only works with BTree.

Basically, just tweaks of https://github.com/louiseGrandjonc/pageinspect_inspector to make it work on me.
