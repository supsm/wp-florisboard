# WP FlorisBoard
Windows Phone theme for [FlorisBoard](https://github.com/florisboard/florisboard). It's not perfect, but I think it's pretty close.  
![WP Dark](https://github.com/supsm/wp-florisboard/assets/60897356/f2b2fb29-7e98-48c1-8c1c-eeb0aa5afd7f)
![WP Light](https://github.com/supsm/wp-florisboard/assets/60897356/a713f6ec-5615-412f-863a-2c888a55fde6)


## Install
1. Install [FlorisBoard](https://github.com/florisboard/florisboard)
2. `Code -> Download ZIP` on Github or `git clone`. Alternatively, use [Github ZIP direct download](https://github.com/supsm/wp-florisboard/archive/master.zip)
3. If you downloaded a .zip, unzip it and enter the extracted folder. `git clone` users should simply enter the local repository directory
4. Create a .zip file of the repository contents. `extension.json`, `stylesheets/`, etc should be at the top level of the .zip file.
5. Open FlorisBoard and go to `Theme -> Manage installed themes -> Import`, then select the .zip file you just created
### FlorisBoard settings
Some things cannot be changed from a theme. Here are some options that can be changed:
- `Keyboard -> Spacebar label` - Current language
- `Keyboard -> Layout -> Key spacing` - 2.0 dp / 2.0 dp
- `Smartbar -> Layout` - Suggestions only
- `Suggestions & Corrections -> Suggestions -> Display suggestions` - ON (nonfunctional as of 0.4.0 but I guess it helps the aesthetic)

Other settings are mostly just personal preference, but there are some things which may make it more similar to Windows Phone behavior.

## Customization
### Accent Color
The accent color is used when a key is pressed, to display caps lock, and the currently selected emoji tab in the emoji screen. The default one is basically a placeholder and can be changed easily. Navigate to `Theme -> Manage installed themes -> Windows Phone Keyboard -> Edit -> Light/Dark -> Edit` and you will find the following relevant variables:
- `--accent-color`: the accent color
- `--accent-color-foreground`: the font color used when the accent color is used as a background (e.g. during keypress and caps lock)
- `--accent-color-glide`: the accent color to use for glide input. This should be the same color as `--accent-color`, but with some transparency. I have found that `0x40` works decently.
### Windows 8 Phone
Navigate to `Theme -> Manage installed themes -> Windows Phone Keyboard -> Edit -> Light/Dark -> Edit` and make the following changes:
- `--key-background`: set to `#474747` for dark and `#ffffff` for light
- `--special-key-background`: set to same values as `--key-background`
