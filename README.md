<h1 align="center">Mak</h1>

<h5 align="center">A piece of paper.</h5>

<div align="center">
  <a href="https://twitter.com/intent/tweet?text=@theinnsinn+A+piece+of+paper:&url=https%3A%2F%2Fmak.ink">
    <img src="https://img.shields.io/twitter/url/https/mak.ink.svg?style=social"/>
  </a>
  <a href="https://gitter.im/inns/mak">
    <img src='https://img.shields.io/gitter/room/inns/mak.svg'/>
  </a>
  <a href="https://github.com/inns/mak">
    <img src='https://img.shields.io/github/package-json/v/inns/mak.svg'/>
  </a>
  <a href="https://mak.ink">
    <img src='https://img.shields.io/website-up-down-green-red/https/mak.ink.svg?label=mak.ink'/>
  </a>
</div>

<img src="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width=880 />

> All you do is sit down at a typewriter and bleed.  
> — Ernest Hemingway

<img src='mak.png' width=128 height=128 align='right'/>


## Table of Contents
- [Features*](#features)
- [Shortcuts](#shortcuts)
- [URL / link](#url--link)
  + [File (#file)](#file-file)
  + [Mode (#file?mode)](#mode-filemode)
  + [URL Action (?action)](#url-action-action)
- [Settings (`set:`)](#settings-set)
- [Developer Console](#developer-console)
- [More Details](#more-details)
  + [LaTeX](#latex)
  + [gist](#gist)
  + [Embeding as iframe](#embeding-as-iframe)
  + [Slideshow (beta)](#slideshow-beta)
  + [Drag and drop](#drag-and-drop)
  + [Desktop App](#desktop-app)
  + [Mobile](#mobile)
  + [iOS App](#ios-app)
  + [Open Source](#open-source)
- [Examples](#examples)
- [Raw Thoughts](#raw-thoughts)
- [Share Mak](#share-mak)
- [License & Acknowledgement](#license--acknowledgement)


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
> **Modes are defined by the URL, and won’t be stored in settings.**  
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
  - [mak.ink?slide](https://mak.ink?slide): open in the slideshow mode
+ Other settings
  - [mak.ink?big](https://mak.ink?big): larger text
  - [mak.ink?cnt](https://mak.ink?cnt): show word counter (as tab title)
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


## Developer Console
[TBD.]


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
Use `?gist=<gist_id>` to load a GitHub gist. It will be stored to `#<gist_id>` automatically (and replace the original context, if exists).  

Note all the `<` and `>` will be replaced due to security reasons. By using `?gist=<gist_id>&xss` you can disable the replacing manually (but it could be dangerous).


### Embeding as iframe
Use **gist** and reading mode:

```html
<iframe width="300" height="200" src="https://mak.ink?gist=5d52fb081b3570c81e3a&read" frameborder="0"></iframe>
```

[TBD.]


### Slideshow<sup>beta<sup>
A modified version of [remark](https://remarkjs.com/) is embeded to enable some slideshow features.

Slides are separated by `---`, checkout the **Examples** section below. And you can find more details in the remark documentation.

Also, this feature is beta currently and there could be unexpected errors.


### Drag and drop
You can drag your file into the editor, and its content will be **inserted** after your cursor automatically.  

Currently all files will be read as **plain text** files. And the file size limit is **10MB**.


### Desktop App
A menubar App as a sticker, no URL stuffs.

Early builds for macOS and Windows: [Mak mini](https://github.com/inns/mak-mini).


### Mobile
For now, all basic features are available in mobile browsers. But there’re yet some known limitations:
- In Safari (macOS or iOS), `localStorage` is disabled in _private browsing mode_.
- In Safari on iOS, the screenshot functionality built on SVG `foreignObject` is not working dut to the iOS security model. So it’s replaced by another, simpler screenshot strategy.
- Service Worker is not fully supported on iOS. The offline feature is not working.

Technique details: due to the slow progress of the [IME](https://caniuse.com/#feat=ime) API implementation on `contenteditable` elements, we are using the native `textarea` as the input handler on mobile devices to make IME work. But textareas cannot do any _styling_ or _customization_. So some implementations in CodeMirror (and any other in-browser editors) might be hacky which caused strange behaviours on mobile devices (such as cursor moving and copy-paste experience). The (only) solution is: make a native App.


### iOS App
WIP. Currently you can add the Web version to your Home screen as a bookmark (data will **not** be synced).

[TBD.]


### Open Source
Will do after some code cleanup & refactoring.


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


## Raw Thoughts
[@chenglou](https://twitter.com/_chenglou) said this in ReactEurope:
> Not about potential power of doing more - it’s about exploiting properties you gain by doing less.

And as I always believe: Text powers editors. Not the opposite.


## Share Mak
[![](https://img.shields.io/twitter/url/https/mak.ink.svg?style=social)](https://twitter.com/intent/tweet?text=@theinnsinn+A+piece+of+paper:&url=https%3A%2F%2Fmak.ink)


## License & Acknowledgement
Powered by [CodeMirror](http://codemirror.net/).

[TBD.]

By Shu (g@shud.in), SH 2017  
https://shud.in
