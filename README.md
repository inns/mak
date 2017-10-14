<img src='https://github.com/quietshu/makpad/raw/master/docs/mak.png' width=200 height=200 align='right'/>

# Mak 
A piece of paper. 

> All you do is sit down at a typewriter and bleed.  
> — Ernest Hemingway


## Features<sup>*</sup>
- a “maximally minimal” look
- multiple notepads
- auto-saving
- offline support
- code highlighting
- LaTeX
- powerful editor
- task lists
- notepad links
- preview mode
- slideshow mode
- quick commands
- UI customization
- line number, word counter
- readable URL configuration
- interactive preferences page & console
- GitHub gist support
- browser zoom friendly
- print friendly (PDF generating)
- screenshot
- data exporting
- ...

<small><sup>*</sup>Some features such as offline and screenshot may act differently in different browsers.</small>


## Shortcuts
> Click (or click with middle mouse button) on Markdown links to open (open in new tab).  
> Click on Markdown checkboxes to toggle a task.  
> Use <kbd>⌘ + [</kbd> / <kbd>⌘ + ]</kbd> to outdent / indent text.  
> Use <kbd>⌥/Alt + Click</kbd> to position the cursor, even on links.  
> Use <kbd>⌘/Ctrl + Click</kbd> to create multiple cursors.  
> Use <kbd>⌥/Alt + Drag</kbd> to select a rectangle area.  
> Use <kbd>⌘/Ctrl + Drag</kbd> to select multiple areas.  
> Use the middle button on mouse to open links in new tab.  
> Type `set:` to open quick commands.  
> Type `go:` to open quick jumping.  


## URL / link
### File (#file)
> Files start with a hashtag `#` in the URL / link.  
> Files can be accessed via in-document links: `[my todos](#todo)`.  
> Files can be accessed via quick jumping: `go:todo` and hit <kbd>enter</kbd>.  

+ Default notepad
  - [mak.ink#](https://mak.ink#): the default notepad
  - [mak.ink](https://mak.ink): or without the hashtag
+ Built-in notepads (**readonly**)
  - [mak.ink#readme](https://mak.ink#readme): documentation
  - [mak.ink#list](https://mak.ink#list): a place to find all your notepads
  - [mak.ink#preferences](https://mak.ink#preferences): preferences
  - [mak.ink#sample](https://mak.ink#sample): the sample document
+ Create your own notepad
  - [mak.ink#whatever_you_want](https://mak.ink#whatever_you_want)


### Mode (#file?mode)
> A mode is a pre-defined way to view files, so modes must be attached to a file.  
> Modes start with a question mark `?` in the URL / link.  
> Multiple modes are separated by `&`s: `mak.ink?dark&big`.  
> **Modes defined by the URL, and won't be stored in settings.**  
> So if you click a link or open another file, current mode will be gone.  
> If you want to use a mode as default option, use settings below.  

+ View modes
  - [mak.ink#sample?edit](https://mak.ink#sample?edit): open sample in editor mode
  - [mak.ink#sample?read](https://mak.ink#sample?read): open sample in reading mode
  - [mak.ink?split](https://mak.ink?split): use split mode in the default notepad
+ Themes
  - [mak.ink?dark](https://mak.ink?dark): dark mode
  - [mak.ink?light](https://mak.ink?light): light mode (default)
+ Slides
  - [mak.ink?slide](https://mak.ink?slide): open in slide mode
+ Other settings
  - [mak.ink?big](https://mak.ink?big): larger text
  - [mak.ink?cnt](https://mak.ink?cnt): show text counter
  - Bascially most of settings can be attached to files as modes.


### URL Action (?action)
> Actions are special modes.  
> Actions start with a question mark `?` in the URL / link,
  and use `=` to pass parameters.  
> Actions will be removed from URL automatically.  
> **Actions might do changes to your content.**  

+ Built-in actions
  - [mak.ink?gist=5d52fb081b3570c81e3a](https://mak.ink?gist=5d52fb081b3570c81e3a): load a gist
+ Combine with modes
  - [mak.ink?gist=5d52fb081b3570c81e3a&read](https://mak.ink?gist=5d52fb081b3570c81e3a&read): load a gist in reading mode


## Settings (`set:<option>`)
> You can type `set:<option>` and hit <kbd>enter</kbd> in the editor to change settings.  
> You can create a "set" link and click on it: `[dark](set:dark)`.  
> Settings change preferences globally and persistently.  
> **Settings can be override (locally) by current modes.**  

+ View mode settings
  - `set:split`
  - `set:edit`
  - `set:read`
+ Display settings
  - `set:dark`
  - `set:light`
  - `set:big`
+ Other
  - `set:print`: print / download PDF
  - `set:img`: take screenshot
+ Other settings
  - Check out the **[Preferences Page](https://mak.ink#preferences)**.
  - You can also use the _developer console_ to change settings :)


## More Details

### LaTeX
The LaTeX rendering feature is powered by [KaTeX](https://khan.github.io/KaTeX/).

You need to wrap the $ inside an inlined code block to render LaTeX inlined equations, or use $$ inside a multi-line code block to get an equation block:  

  `$\frac{\pi}{2}$`

or

  ```
  $$
  \frac{\pi}{2}
  $$
  ```


### gist
Use `?gist=<gist_id>` to load a GitHub gist. It will be stored to `#<gist_id>` automatically.  

Note all the `<` and `>` will be replaced due to security reasons. By using `?gist=<gist_id>&xss` you can disable the replacing manually (but it could be dangerous).

[TBD.]

### Slideshow <sup>beta<sup>
A modified version of [remark](https://remarkjs.com/) is embeded to enable some slideshow features.

[TBD.]

### Drag and drop
You can drag your file into the editor, and its content will be **inserted** after your cursor automatically.  

Currently all files will be read as **plain text** files. And the file size limit is **10MB**.


### Quote placeholders
[TBD.]


### iOS browser
[TBD.]


### iOS App
[TBD.]


### Desktop App
A menubar App as a sticker, no URL stuffs.

Early builds for macOS and Windows: [Mak mini](https://github.com/quietshu/makpad-mini).


## Examples

+ Read a file
  - [mak.ink#sample?read](https://mak.ink#sample?read)
  - [mak.ink#sample?read&nomath](https://mak.ink#sample?read&nomath)
+ gist
  - [mak.ink?gist=5d52fb081b3570c81e3a&read](https://mak.ink?gist=5d52fb081b3570c81e3a&read)
  - [mak.ink?gist=cf1925eed030c77bd0941b2e65e40f51&split&xss](https://mak.ink?gist=cf1925eed030c77bd0941b2e65e40f51&split&xss)
+ gist + slideshow
  - [mak.ink?gist=3177ebc6b01dcfaf555c153f601ebf94&slide](https://mak.ink?gist=3177ebc6b01dcfaf555c153f601ebf94&slide)
  - [mak.ink?gist=3177ebc6b01dcfaf555c153f601ebf94&slide&edit](https://mak.ink?gist=3177ebc6b01dcfaf555c153f601ebf94&slide&edit)
  - You can easily share a document / slide to others by using these URL schemas on gists.  


## Raw thoughts
[@chenglou](https://twitter.com/_chenglou) said this in ReactEurope:
> Not about potential power of doing more - it's about exploiting properties you gain by doing less. 

As I always believe: Text powers editors. Not the opposite.


## License & Acknowledgement
[TBD.]

By Shu (g@shud.in), SH 2017  
https://shud.in