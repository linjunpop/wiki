# Tips

## Clear 'Open with...'

http://apple.stackexchange.com/a/68600/23966

```bash
$ /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/LaunchServices.framework/Versions/A/Support/lsregister -kill -r -domain local -domain system -domain user
```

## Free inactive Memory

http://osxdaily.com/2012/04/24/free-up-inactive-memory-in-mac-os-x-with-purge-command/

```bash
$ purge
```