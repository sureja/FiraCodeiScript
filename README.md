# Fira Code iScript

A font mashup to be used in code editors, displaying a script typeface for the italic font style.

The Regular and Bold face styles are taken from [Fira Code](https://github.com/tonsky/FiraCode) and [Script12](https://www.myfontsfree.com/134618/script12pitchbt.htm).

![image](https://user-images.githubusercontent.com/7041191/30752845-8c8484ce-9f8b-11e7-9df1-1d171b8d5e66.png)
![image](https://user-images.githubusercontent.com/7041191/30753423-41be3e06-9f8d-11e7-930d-9cfdb5b5ee60.png)
![image](https://user-images.githubusercontent.com/7041191/30752894-b5ff4b4a-9f8b-11e7-9908-969829409d08.png)

## Install

Download or clone this repository and install the fonts on your system.

In your editor of choice set the font to `Fira Code iScript`.  Also, ensure that the current theme and syntax highlighting utilize italic.


### Also refer this stack overflow page to edit user settings.json 

https://stackoverflow.com/questions/41320848/how-do-i-get-visual-studio-code-to-display-italic-fonts-in-formatted-code/50714195#50714195 

```
"editor.tokenColorCustomizations": {
  "textMateRules": [
    {
      "scope": [
        //following will be in italic (=FlottFlott)
        "comment",
        "entity.name.type.class", //class names
        "keyword", //import, export, return…
        "constant", //String, Number, Boolean…, this, super
        "storage.modifier", //static keyword
        "storage.type.class.js", //class keyword
      ],
      "settings": {
        "fontStyle": "italic"
      }
    },
    {
      "scope": [
        //following will be excluded from italics (VSCode has some defaults for italics)
        "invalid",
        "keyword.operator",
        "constant.numeric.css",
        "keyword.other.unit.px.css",
        "constant.numeric.decimal.js",
        "constant.numeric.json"
      ],
      "settings": {
        "fontStyle": ""
      }
    }
  ]
}

```
