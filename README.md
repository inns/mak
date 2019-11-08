<p align="center">
  <img src='mak.png' width=128 height=128 align='center'/>
</p>

<h3 align="center"><b>Mak: a universal notepad</b></h3>

<p align="center">
  <a href="https://mak.ink">mak.ink</a>&nbsp;&nbsp;&nbsp;
  <a href="#desktop-app">Desktop App</a>&nbsp;&nbsp;&nbsp;
  <a href="https://inns.studio/mak">Documentation</a>&nbsp;&nbsp;&nbsp;
  <a href="https://twitter.com/shuding_">@shuding_</a>
  <br/>
  <br/>
</p>

<div align="center">
  <a href="https://twitter.com/intent/tweet?text=@theinnsinn+A+piece+of+paper:&url=https%3A%2F%2Finns.studio%2Fmak">
    <img src="https://badgen.net/badge/Share/tweet?icon=twitter"/>
  </a>
  <a href="https://mak.ink">
    <img src='https://badgen.net/uptime-robot/day/m780777417-1f8362b19452b5fe087b4c7f'/>
  </a>
</div>

<img src="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width=880 />

> All you do is sit down at a typewriter and bleed.  
> — Ernest Hemingway

**Please visit https://inns.studio/mak for more information and live demos.** 

Join [Mak User Group](https://t.me/mak_ink) ([中文用户群](https://t.me/mak_ink_cn)) on Telegram.

## Table of Contents
- [Features*](#features)
- [Shortcuts](#shortcuts)
- [URL / link](#url--link)
  + [File (#file)](#file-file)
  + [Mode (#file?mode)](#mode-filemode)
  + [URL Action (?action)](#url-action-action)
- [Settings (`set:`)](#settings-set)
- [More Details](#more-details)
  + [LaTeX](#latex)
  + [Gist](#gist)
  + [Embeding as iframe](#embeding-as-iframe)
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
- a “maximally minimal” design
- blazing fast
- multiple files support
- auto-saving
- works in offline
- side by side preview
- syntax highlighting
- powerful text editor
- LaTeX support
- task lists
- notepad links
- quick commands
- customization
- line number
- word counter
- URL configuration
- interactive plain text
- sync via Gists
- zoom friendly
- printer friendly
- PDF generating
- exporting
- ...

<small><sup>*</sup>Some features such as offline and sync may behave differently in different browsers.</small>


## Shortcuts
> Click (or click with middle mouse button) on Markdown links to open (open in new tab).  
> Click on Markdown checkboxes to toggle a task.  
> Use <kbd>⌘ + [</kbd> / <kbd>⌘ + ]</kbd> to outdent / indent text.  
> Use <kbd>⌥/Alt + Click</kbd> to position the cursor, even on links.  
> Use <kbd>⌘/Ctrl + Click</kbd> to create multiple cursors.  
> Use <kbd>⌥/Alt + Drag</kbd> to select a rectangle area.  
> Use <kbd>⌘/Ctrl + Drag</kbd> to select multiple areas.  
> Use the middle button on mouse to open links in new tab.  
> Use <kbd>⌘/Ctrl + Enter</kbd> over a link to “click” it.
> Type `set:` to open quick commands.  
> Type `go:` to open quick jump.  


## URL / link
### File (#file)
> Files start with a hashtag `#` in the URL / link.  
> Files can be accessed via in-document links: `[my todos](#todo)`.  
> Files can be accessed via quick jump: `go:todo` and hit <kbd>enter</kbd>.  

+ Default file
  - [mak.ink#](https://mak.ink#): the default file
  - [mak.ink](https://mak.ink): without the hashtag
+ Built-in notepads (**readonly**)
  - [mak.ink#list](https://mak.ink#list): a place to find all your files
  - [mak.ink#preferences](https://mak.ink#preferences): preferences
  - [mak.ink#sample](https://mak.ink#sample): the sample document
  - [mak.ink#profile](https://mak.ink#profile): user profile
+ Create a file
  - [mak.ink#whatever_you_want](https://mak.ink#whatever_you_want)


### Mode (#file?mode)
> A mode is a pre-defined way to view files, so modes must be attached to a file.  
> Modes start with a question mark `?` in the URL / link.  
> Multiple modes are separated by `&`s: `mak.ink?dark&large`.  
> **Modes are defined by the URL, and will override your settings.**  
> For new opened files, modes attached to current file will be gone.  
> If you want to use a mode as default option, use settings below.  

+ View modes
  - [mak.ink#sample?edit](https://mak.ink#sample?edit): open sample in editor mode
  - [mak.ink#sample?read](https://mak.ink#sample?read): open sample in reading mode
  - [mak.ink?split](https://mak.ink?split): use split mode in the default notepad
+ Themes
  - [mak.ink?dark](https://mak.ink?dark): dark mode
  - [mak.ink?light](https://mak.ink?light): light mode (default)
+ Other settings
  - [mak.ink?large](https://mak.ink?large): larger text
  - [mak.ink?num](https://mak.ink?num): show line number
+ Combine
  - [mak.ink?dark&large](https://mak.ink?dark&large)


### URL Action (?action)
> Actions are special modes.  
> Actions start with a question mark `?` in the URL / link,
  and use `=` to pass parameters.  
> Actions will be removed from URL automatically.  
> **Actions might do changes to your content.**  

+ Built-in actions
  - [mak.ink?gist=5d52fb081b3570c81e3a](https://mak.ink?gist=5d52fb081b3570c81e3a): load a Gist and create a file (#5d52fb081b3570c81e3a)
+ Combine modes
  - [mak.ink?gist=5d52fb081b3570c81e3a&read](https://mak.ink?gist=5d52fb081b3570c81e3a&read): load a Gist in reading mode


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
  - `set:large`
+ Other
  - `set:print`: print / download PDF
  - `set:export`: export data
+ Other settings
  - Check out the **[Preferences Page](https://mak.ink#preferences)**.
  - You can also use the _developer console_ to change settings :)


## More Details

### LaTeX
LaTeX rendering is powered by [KaTeX](https://khan.github.io/KaTeX/).

You need to wrap the $ inside an inlined code block to render LaTeX inlined equations, or use $$ inside a multi-line code block to get an equation block:  

  `$\frac{\pi}{2}$`

or

  ```
  $$
  \frac{\pi}{2}
  $$
  ```


### Gist
Use `?gist=<gist_id>` to load a GitHub Gist. It will be stored to `#<gist_id>` automatically (and replace the original context, if it exists), and mark this file as a Gist.  

Other commands: `set:login`, `set:logout`, `set:pull`, `set:push`.


### Embeding as iframe
Use **Gist** and read mode:

```html
<iframe width="300" height="200" src="https://mak.ink?gist=5d52fb081b3570c81e3a&read" frameborder="0"></iframe>
```

You can easily embed Mak in other websites.


### Drag and drop
You can drag your file into the editor, and its content will be **inserted** after your cursor automatically.  

Currently all files will be read as **plain text** files. And the file size limit is **10MB**.


### Desktop App
Checkout [Mak<sup>mini</sup>](https://github.com/inns/mak-mini) for macOS and Windows.


### Mobile
*Currently unavailable.*

For now, all basic features are available in mobile browsers. But there’re yet some known limitations:
- In Safari (macOS or iOS), `localStorage` is disabled in _private browsing mode_.
- In Safari on iOS, the screenshot functionality built on SVG `foreignObject` is not working dut to the iOS security model. So it’s replaced by another, simpler screenshot strategy.
- Service Worker is not fully supported on iOS. The offline feature is not working.

Technique details: due to the slow progress of the [IME](https://caniuse.com/#feat=ime) API implementation on `contenteditable` elements, we are using the native `textarea` as the input handler on mobile devices to make IME work. But textareas cannot do any _styling_ or _customization_. So some implementations in CodeMirror (and any other in-browser editors) might be hacky which caused strange behaviours on mobile devices (such as cursor moving and copy-paste experience). The (only) solution is: make a native App.


### iOS App
*Currently unavailable.*

WIP. You can add the Web version to your Home screen as a bookmark.


### Open Source
Will do after some code cleanup & refactoring.


## Raw Thoughts
[@chenglou](https://twitter.com/_chenglou) said this in ReactEurope:
> Not about potential power of doing more - it’s about exploiting properties you gain by doing less.

And as I always believe: Text powers editors. Not the opposite.


## Share Mak
[![](https://badgen.net/badge//twitter?icon=twitter)](https://twitter.com/intent/tweet?text=@theinnsinn+A+piece+of+paper:&url=https%3A%2F%2Finns.studio%2Fmak)


## License & Acknowledgement
Inspired and powered by [CodeMirror](http://codemirror.net/), [RxJS](https://github.com/Reactive-Extensions/RxJS) and other awesome open source projects.


By Shu (g@shud.in), SH 2017  
https://shud.in
