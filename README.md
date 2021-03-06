# Neutrality - A light theme, with balanced colors to minimize eye strain

## Supported Languages 
Polished support for ES6 (JavaScript), HTML, CSS, SCSS, Markdown, JSON. General support for most other languages, based on the colors used for JavaScript.

## About **Neutrality**

**Neutrality** is a darker version of [Daobeam][1], with modified foreground colors.

All colors are meant to compliment each other. I have attempted to harmonize colors using [a professional tool][0].

CSS: Property values are all the same color (good!).

Comments: Consistent contrast level compared to other code. Theme designers: we already understand that comments are not processed as code. We don't need a visual indication (making them ultra-low contrast, etc.). **We should be able to read comments just as easily as code!**

I am open to pull requests and constructive feedback. I would like to see polished support for many other languages, particularly back-end languages. If you like **Neutrality**, please review it.

## User Settings Recommendations
VS Code user settings has properties to increase the font-size of the source code (`editor.fontSize`), the terminal (`terminal.integrated.fontSize`), but *not* the editor sidebar. Here is a workaround for this limitation: Increase the overall font-size of everything using `window.zoomLevel`, and then slightly *decrease* the `editor.fontSize` and `terminal.integrated.fontSize` to compensate for increasing `window.zoomLevel`:

```
{
    "workbench.colorTheme": "Neutrality",
    "editor.fontFamily": "Consolas",
    "editor.wordWrap": "on",
    "files.autoSave": "onFocusChange",
    
    //BEGIN these settings work in tandem ~~~~~~~~
    "window.zoomLevel": 0.7, // 0.7<-- keep this value in a comment, because it will be overwritten on ctrl + 0, ctrl + +, or ctrl + -.
    "editor.fontSize": 16, // smaller than I would want it if window.zoomLevel was 0
    "terminal.integrated.fontSize": 15, //smaller than I would want it if window.zoomLevel was 0
    //END these settings work in tandem ~~~~~~~~    
}
```
## Pay it Forward at World Community Grid
Please join the [Daobeam World Community Grid team](https://join.worldcommunitygrid.org?teamId=RF7TGV6H72). Just sign up, download the software, and start crunching.

## License
GNU General Public License v3.0

## Enjoy **Neutrality**!

[0]:https://www.sessions.edu/color-calculator/

[1]:https://marketplace.visualstudio.com/items?itemName=mike-flanigan.Daobeam

[7]:https://join.worldcommunitygrid.org?teamId=RF7TGV6H72
