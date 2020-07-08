# Notepad++ custom syntax highlighters

[What is Notepad++](https://notepad-plus-plus.org/)

[Supported programming languages in Notepad++](https://npp-user-manual.org/docs/programing-languages/)

## How to use
1. Download the language files you want
1. Open an Explorer window and go to `%appdata%\Notepad++\userDefineLangs`
1. Copy (or move) the previously downloaded XML files right there
1. (close and re)Open Notepad++ to see the new languages available
1. (Optional) Select the highlighting language manually

## Custom language syntax highlighting

[Syntax highlighters from the community](https://github.com/notepad-plus-plus/userDefinedLanguages/tree/master/UDLs)

[UDL documenation](https://npp-user-manual.org/docs/user-defined-language-system/)

[Unofficial UDL documentation](http://ivan-radic.github.io/udl-documentation/)

[Style configurator](https://npp-user-manual.org/docs/preferences/#style-configurator)

## Supported languages

### Markdown
What is done right:
- "Light" version is for light themes. The colors are from the default Notepad++ theme.
- "Dark" version is for dark themes. The colors are from the Zenburn theme.
- The text background is kept transparent => compatibility with more than one theme.
- The text style is overrided only if needed => compatibility with more than one theme.
- Any title levels are supported.
- Bold and italic styling doesn't stop at first word.

Known limitations:
- Strikethrough text is rendered with a different color, because Notepad++ doesn't support ~~strikethrough~~ styling.
- The use of underscores in URLs can generate unwanted italic texts like in this example: [ image ] (https://github.com/test_image.png _"This text is italic whereas it should not")_ (from `[ image ] (https://github.com/test_image.png "This text is italic whereas it should not")`)
- Nesting italic inside bold or bold inside italic won't combine styles.\
`**this _is my_ text**` will render '**this** _is my_ **text**' (instead of '**this _is my_ text**').

### smartBASIC
Language used by Laird Technologies.

### Spice
Language used by the SPICE simulation engine.

## Notes about the User Defined Languages (UDL)

- `fgColor` = foreground color (= text color)
- `bgColor` = text _background_ color

### The 'colorStyle' property
value | caption | description
----- | ------- | -----------
0 | default | use the default fgColor and bgColor
1 | fgColor | use the provided fgColor, and the default bgColor
2 | bgColor | use the provided bgColor, and the default fgColor
3 | both | use the provided fgColor and bgColor

### The 'fontStyle' property
value | font style
----- | ----------
0 | standard
1 | bold
2 | italic
3 | bold + italic
4 | underlined
5 | bold + underlined
6 | italic + underlined
7 | bold + italic + underlined
