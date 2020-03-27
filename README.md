# Notepad++ custom syntax highlighters

[What is Notepad++](https://notepad-plus-plus.org/)

## Notes about the User Defined Languages (UDL)

[Unofficial UDL documentation](http://ivan-radic.github.io/udl-documentation/)

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
1 | **bold**
2 | *italic*
3 | ***bold + italic***
4 | underlined
5 | bold + underlined
6 | italic + underlined
7 | bold + italic + underlined
