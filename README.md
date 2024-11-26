# MinimalResoniteRunnerTemplate

(most of difficult stuff here was discovered by whatsavalue3, so credit should go to them)

This is a minimal template, useful to call Resonite code (including world stuff) via an application that links to the User's Resonite exe

The main goal of this is a single exe with minimal dependencies (not even Resonite dependencies!) that'll load 
a Resonite world locally which can then be modified with code. Connecting to other users isn't supported,
this is intended for use in a Unity Exporter I made but figured it might be of use to others as well.

How it works is you run it, then provide it the location of your Resonite.exe. It'll then use the libraries
there to dynamically load from FrooxEngine and SkyFrost etc. and host a private world.

By not baking in links to Resonite directly, it's more likely this should stay compatible as Resonite changes over time.

## Credits:

- Thanks to whatsavalue3 for most of the code needed to run Resonite (I just tweaked it a bit and made it dynamically call Resonite dlls)
- Thanks to [https://github.com/Lexevolution/Resonite-DataTree-Converter](Lexevolution) for dynamically loading Resonite dlls code that I modified