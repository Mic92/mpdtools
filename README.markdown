mpdmark
=======

requirements:
----------
- python

- python-mpd

- mpd v0.15 or greater (need sticker support)

```
usage: mpdmark [-h] [--host HOST] [--port PORT] [--password PASSWORD]
               {list,del,save,load} ...

Bookmark song position in mpd

positional arguments:
  {list,del,save,load}
    list                list all bookmarks
    del                 delete a bookmark
    save                save postion of current song
    load                load the last bookmark

optional arguments:
  -h, --help            show this help message and exit
  --host HOST           Host address to connect to.
  --port PORT           Port to connect to.
  --password PASSWORD   Host address to connect to.
```

mpdadd
======

requirements:
----------
- ruby

- librmpd (avaible as gem)

- ruby-gtk (optional, to use the file dialog)

- needs direct access to mpd's music path to create links

```
usage: mpdadd [options] files...
Add songs from outside of your mpd library to your playlist

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
