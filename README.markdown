mpdmark
=======

depencies:
----------
- python

- python-mpd

```
usage: mpdmark [-h] {list,del,save,load} ...

Bookmark song position in mpd

positional arguments:
  {list,del,save,load}
    list                list all bookmarks
    del                 delete a bookmark
    save                save postion of current song
    load                load the last bookmark

optional arguments:
  -h, --help            show this help message and exit
```

mpdadd
======

depencies:
----------
- ruby

- librmpd (avaible as gem)

```
usage: mpdadd [options] files...
Add all songs on your harddrive to your local MPD

Specific options:
        --host                       the host to connect to [default: localhost]
        --port                       the port to connect to [default: 6600]
    -g, --gui                        Use a gui file dialog (requires ruby-gtk) [default: off]
    -l, --library [DIRECTORY]        Play the first file added immediately [default: ~/music]
    -p, --play                       Play the first file added immediately [default: off]
    -s, --save                       Save current options to file '~/.mpdadd'
    -h, --help                       Show this help.
    -v, --[no-]verbose               Logging verbosely [default: off]
```