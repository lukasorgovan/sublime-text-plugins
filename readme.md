# Good Sublime Text 2 plugins

This is list of all packages (plugins) I use in my projects. Some of them more often, some not so often. All of them are very good and work as expected.

* [Emmet](http://docs.emmet.io/) - syntax abbreviation expander, saves so much time when creating mockups
* [Prefixr](http://wbond.net/sublime_packages/prefixr) - MUST HAVE for every developer. No need to remeber all those prefixes, Prefixr plugin communicates directly through [Nettuts Prefixr API](http://prefixr.com/)
* [Docblockr](https://github.com/spadgos/sublime-jsdocs) - generates documentation automatically
write `/**` and press `Enter` or `Tab`. You will get block comment. If the line direclty afterwards contains a function definition, parameters and function name will be added. Check [documentation](https://github.com/spadgos/sublime-jsdocs)
* [Markdown preview](https://github.com/revolunet/sublimetext-markdown-preview) - wonderfull plugin for reading .MD files from. It even contains Markdown CheatSheet!
* [JSHint](http://www.jshint.com/install/) - you need to have Node.js installed. Then you can easily install JSHint via terminal `npm install -g jshint`
* [Aqua Color Theme](https://github.com/cafarm/aqua-theme) - I prefer the ProKit variation with Tomorrow Night Aqua color scheme but [hey! there are many beautiful color schemes out htere](https://github.com/daylerees/colour-schemes)
* Colorpicker - opens native OS color picker
## My preferences

```
{
	"color_scheme": "Packages/Theme - Aqua/Color Schemes/Tomorrow Night Aqua.tmTheme",
	"font_face": "Monaco",
	"font_options":
	[
		"gray_antialias" 
	],
	"font_size": 14.0,
	"ignored_packages":
	[
		"Vintage"
	],
	"tab_size": 2,
	"theme": "ProKit.sublime-theme"
}
```
## How to sync your plugins (packages) AND preferences accross multiple computers
Probably the best is to use Dropbox folder and make symlinks

[How-to sync](http://misfoc.us/post/18018400006/syncing-sublime-text-2-settings-via-dropbox) **for Windows users**

1. Quit Sublime Text 2
2. In your Dropbox folder create new folder called Sublime Text 2
3. Open the folder with your sublime settings (should be `~/Library/Application Support/Sublime\ Text\ 2/`)
4. Copy the following 3 folders into `~/Dropbox/Sublime\ Text\ 2/`: `Installed Packages`, `Packages`, and `Pristine Packages`
5. Rename those folders in Application Support for backup reasons
5. With your Terminal cd into ~/Library/Application\ Support/Sublime\ Text\ 2/ 
6. Create symlinks to Dropbox using later syntax

```
  ln -s ~/Dropbox/Sublime\ Text\ 2/Installed\ Packages ./Installed\ Packages
  ln -s ~/Dropbox/Sublime\ Text\ 2/Packages ./Packages
  ln -s ~/Dropbox/Sublime\ Text\ 2/Pristine\ Packages ./Pristine\ Packages
```