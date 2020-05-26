# Spring 2020 SSSO on-stream graphics

A "small" guide on how to set up the on-stream graphics for your own Spin Rhythm related tournaments!

[Trello board](https://trello.com/b/8i1AGQMJ/spring-2020-sso-on-stream-graphics/)

## Prerequisites

- [OBS](https://obsproject.com)
  - Plugins:
    - [Spectralizer](https://obsproject.com/forum/resources/spectralizer.861/)
    - [StreamFX](https://obsproject.com/forum/resources/streamfx-for-obs-studio.578/)
  - [VLC](https://www.videolan.org/vlc/index.html/)
  - [Foobar](https://www.foobar2000.org/)
    - [Foobar NP Simple plugin](https://skipyrich.com/w/index.php/Foobar2000:Now_Playing_Simple/)
  - [Snaz](https://github.com/JimmyAppelt/Snaz/wiki/)
  - Not neccesary:
    - [ImBatch](http://www.highmotionsoftware.com/products/imbatch/)
    - [Chatty](https://chatty.github.io/)

## OBS Setup

### How to import scenes and profiles

  Open OBS studio, after opening OBS studio, go to `Profile` -> `Import` and select the `Tournament2` folder in `\Spring2020SSSOgraphics\OBS\`
  
  Now it's time to import the Scene Collection. Go to `Scene Collection` -> `Import` and click no on any popups that may appear. Now the `Scene Collection Importer` window should be open.
  ![Scene Collection Importer](https://puu.sh/FP5ax/e38e5c8d46.png)
  
  Click on `Add` and select the `Tournament.json` file in `\Spring2020SSSOgraphics\OBS\`, then click on Import. 
  You should now have a `Tournament` Scene Collection under the `Scene Collection` tab.

  Make sure you are on the right `Profile` and `Scene Collection` before going any further.

### How to fix sources and filters

#### Sources

  After importing both the `Scene Collection` and the `Profile` you will most likely notice that most things look kinda black, with nothing on screen, you will have to go through all the sources and locate the files, they are named the same.

  For example: ![example](https://puu.sh/FP6k2/7784697ed2.png)
  ![example2](https://puu.sh/FP6mj/43360451b3.png)

  Do this for all sources that appear to need a local file. Ignore files that point to `C:/Users/thomt/AppData/Roaming/Tapstream/...`. We'll come back to these in the `Tapstream How-to`.

#### Filters

  Now, we'll have to check all the source's filters, right click a source and click on `Filters`

  For example, the `Tapstream` source has an `Image Mask/Blend` this requires the file `maskquestion.png` ![maskquestion.png](https://puu.sh/FP6AY/cb942adaf1.png)

  We'll also have to relocate these files, the same way we did for the `Sources`. Make sure you check every source for filters.

#### Transition

  Make sure to place the `Transition 9.webm` file from `\Spring2020SSSOgraphics\graphics\` in `C:/Users/"yourusername"/AppData/Roaming/obs-studio/transitions/` and update the path in the properties for `stinger 9`
  ![stinger 9 properties](https://puu.sh/FP8R2/e3ec12c836.png)

#### Final

  After setting all these to the correct file locations. Your OBS should look a lot more lively!

### The OBS keybinds

#### Switch to scene: TOURNAMENT

*key combo* - <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>Shift</kbd> + <kbd>F1</kbd>

#### Switch to scene: Stats

*key combo* - <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>Shift</kbd> + <kbd>F2</kbd>

#### Switch to scene: countdown/brackets

*key combo* - <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>Shift</kbd> + <kbd>F3</kbd>

#### Switch to scene: Transition (***DON'T USE THIS***)

*key combo* - <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>Shift</kbd> + <kbd>F4</kbd>

#### Mute `Gamer 1` and unmute `Gamer 5 (2)`*

*key combo* - <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>Num 2</kbd>

#### Mute `Gamer 5 (2)` and unmute `Gamer 1`*

*key combo* - <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>Num 1</kbd>

##### * muting and unmuting `Gamer 1` and `Gamer 5 (2)` automatically changes the hidden/shown status of `vol-1` and `vol-2`
