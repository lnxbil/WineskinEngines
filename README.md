# No-Flickering Wineskin Engines
Here you have a built of a non-flickering [Wineskin](http://wineskin.urgesoftware.com/tiki-index.php) engine.

As stated in [Wine Bug](http://bugs.winehq.org/show_bug.cgi?id=34166), there is a [Patch from Linus Unnebäck for 1.7.4](http://bugs.winehq.org/attachment.cgi?id=46394&action=edit), which does not apply directly to the new wine version 1.7.11.

I patched the patch to work with 1.7.11 and you can download it directly from this repository. There is also a prebuilt engine for Wineskin.

To use the prebuilt engine, please copy [this file](https://github.com/lnxbil/WineskinEngines/raw/master/WS9Wine1.7.11NoFlicker.tar.7z) to

    $HOME/Library/Application Support/Wineskin/Engines

The Engine was built on a freshly installed *Mac OS Snow Leopard* with included XCode. The log is also [available](https://github.com/lnxbil/WineskinEngines/raw/master/WS9Wine1.7.11NoFlicker.build.log.rtf).

## Easy installation

Copy and paste the following line into a terminal window, then hit enter.

```sh
curl -L "https://raw2.github.com/lnxbil/WineskinEngines/master/WS9Wine1.7.11NoFlicker.tar.7z" > "$HOME/Library/Application Support/Wineskin/Engines/WS9Wine1.7.11NoFlicker.tar.7z"
```

This engine will then show up in the list of engines in Wineskin Winery as `WS9Wine1.7.11NoFlicker`.
