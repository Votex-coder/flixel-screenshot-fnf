<div align="center">

# flixel-screenshot-fnf

## `haxelib git flixel-screenshot-plugin http://github.com/sayofthelor/flixel-screenshot-plugin`

</div>

## Flixel plugin for nice screenshot management, with many customizations
```haxe
ScreenShotPlugin.enabled:Bool; // Enable/disable the plugin at any time
ScreenShotPlugin.screenshtotKeys:Array<FlxKey>; // Keys to press to do a screenshot
ScreenShotPlugin.saveFormat:FileFormatOption; // The save file type (FileFormatOption.PNG/ FileFormatOption.JPEG)
ScreenShotPlugin.screenshotPath:String; // The path where to save the screenshots
ScreenShotPlugin.flashColor:Int; // The color of the flash that appears when taking a screenshot (0xAARRGGBB)
ScreenShotPlugin.outlineColor:Int; // The shot display outline's color that appears when taking a screenshot (0xAARRGGBB)
ScreenShotPlugin.screenshotFadeTime:Float; // The flash fade-in duration
ScreenShotPlugin.screenshot(); // Screenshot your game of script(lua)/code(hx) 
ScreenShotPlugin.jpegQuality:Int; // If `saveFormat` is set to JPEG, this defines the quality of the JPEG files (0-100)
ScreenShotPlugin.sound:FlxSoundAsset; // Custom sound asset to play when the screenshot is taken (if null, no sound is played)
```

### Some original code from [flixel-addons](http://lib.haxe.org/p/flixel-addons).

### Original plugin [flixel-screenshot-plugin](https://lib.haxe.org/p/flixel-screenshot-plugin)

# Configuring
Make sure you have `flixel` and `openfl` installed.
In your `Project.xml` make sure this is there:
```xml
<haxelib name="flixel-screenshot-fnf" />
```
In your project's `Main.hx` file, after the `FlxGame` is initialized, add this line:
```haxe
flixel.FlxG.plugins.add(new flixel.addons.plugin.ScreenShotPlugin());
```
And you're done!
