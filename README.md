# No-Flickering Wineskin Engines
Here you have a couple of unoffical [Wineskin](http://wineskin.urgesoftware.com/tiki-index.php) engines for [Wine Bug #34166](http://bugs.winehq.org/show_bug.cgi?id=34166):

* ```WS9Wine1.7.11``` - Vanilla Wine Version (**has** flickering bug, only for reference)
* ```WS9Wine1.7.11-noflicker-unnebäck``` - [Patch by Linus Unnebäck for 1.7.4](http://bugs.winehq.org/attachment.cgi?id=46394&action=edit)
* ```WS9Wine1.7.11-noflicker-verbeet``` - [Patch by Henri Verbeet for 1.7.11](http://bugs.winehq.org/attachment.cgi?id=47352&action=edit)

I patched the patch from Linux Unnebäck to work with 1.7.11 and you can download it directly from this repository.

Benchmark results using all three engines are available [here](https://github.com/lnxbil/WineskinEngines/tree/master/Benchmark-1.7.11).

The engines were built on a freshly installed *Mac OS Snow Leopard* with included XCode. I used a different format for naming the engines (**-** after wine version) to make it clear that they're not officially approved.

## Easy installation

Copy and paste the following line into a terminal window, then hit enter (please see also next section to activate it).

*  Verbeet engine (Fixing `Double Buffering Issue`):

   ```sh
curl -L "https://raw2.github.com/lnxbil/WineskinEngines/master/WS9Wine1.7.11-noflicker-verbeet.tar.7z" > "$HOME/Library/Application Support/Wineskin/Engines/WS9Wine1.7.11-noflicker-verbeet.tar.7z"
   ```

   This engine will then show up in the list of engines in Wineskin Winery as `WS9Wine1.7.11-noflicker-verbeet`.

*  Unnebäck engine (Disabled `updateColorSpace`):

   ```sh
curl -L "https://raw2.github.com/lnxbil/WineskinEngines/master/WS9Wine1.7.11-noflicker-unneback.tar.7z" > "$HOME/Library/Application Support/Wineskin/Engines/WS9Wine1.7.11-noflicker-unnebäck.tar.7z"
   ```

   This engine will then show up in the list of engines in Wineskin Winery as `WS9Wine1.7.11-noflicker-unnebäck`.

## Activate inside Wineskin
To activate the new engine, you have to use the _Native Driver_ under _Screen Options_. Please check if the following is enabled:

    X   Use Mac Driver instead of X11
    
as it is shown on this screenshot:

![Screenshot](https://github.com/lnxbil/WineskinEngines/raw/master/screen_options.png)

## Patches
The patches for the corresponding versions can also be downloaded here:

* [WS9Wine1.7.11-noflicker-verbeet.diff](https://raw2.github.com/lnxbil/WineskinEngines/master/WS9Wine1.7.11-noflicker-verbeet.diff)
* [WS9Wine1.7.11-noflicker-unneback.diff](https://raw2.github.com/lnxbil/WineskinEngines/master/WS9Wine1.7.11-noflicker-unneback.diff)
