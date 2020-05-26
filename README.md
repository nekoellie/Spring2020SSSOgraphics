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
  #### How to import scenes and profiles
  Open OBS studio, after opening OBS studio, go to `Profile` -> `Import` and select the `Tournament2` folder in `\Spring2020SSSOgraphics\OBS\`
  
  Now it's time to import the Scene Collection. Go to `Scene Collection` -> `Import` and click no on any popups that may appear. Now the `Scene Collection Importer` window should be open.
  ![Scene Collection Importer](https://puu.sh/FP5ax/e38e5c8d46.png)
  Click on `Add` and select the `Tournament.json` file in `\Spring2020SSSOgraphics\OBS\`, then click on Import. 
  You should now have a `Tournament` Scene Collection under the `Scene Collection` tab.

  Make sure you are on the right `Profile` and `Scene Collection` before going any further.