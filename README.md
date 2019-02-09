# Github Markdown Snippets

Markdown files on github can be styled using either github flavored markdown or with certain html tags and attributes. These snippets should serve as a cheatsheet and a reference list of several different techniques.

<table><tbody><tr>
<td><details><summary>Table of Contents</summary>

1. [Basic Formatting](#basic-formatting)
   1. [Headers](#headers)
   2. [Italics](#italics)
   3. [Bold](#bold)
   4. [Strikethrough](#strikethrough)
   5. [Links](#links)
   6. [Code](#code)
   7. [Quotes](#quotes)
   8. [Tables](#tables)
   9. [Lists](#lists)
   10. [Images](#images)
2. [HTML](#html)
   1. [Tags](#tags)
   2. [Attributes](#attributes)
   3. [Entities](#entities)
   4. [Emojis](#emojis)
3. [Text](#text)
   1. [Subscripts](#subscripts)
   2. [Superscripts](#superscripts)
4. [Alignments](#alignments)
   1. [Center Aligned](#center-aligned)
   2. [Right Aligned](#right-aligned)
   3. [Split Page](#split-page)
   4. [Triple Alignment](#triple-alignment)
5. [Images](#images)
   1. [Specify Size](#specify-size)
6. [Style](#style)
   1. [Surround by Box](#surround-by-box)
   2. [Divider Line](#divider-line)
   3. [Hotkey Styling](#hotkey-styling)
   4. [Dropdown / Collapsing / Spoilers](#dropdown--collapsing--spoilers)
   5. [Start-of-line Asterisk](#start-of-line-asterisk)
7. [Composed](#composed)
   1. [Table of Contents](#table-of-contents)
   2. [Captioned Image](#captioned-image)
</details></td>
</tr></tbody></table>

## Basic Formatting

### Headers

```
# 1
## 2
### 3
#### 4
##### 5
###### 6
```

# 1
## 2
### 3
#### 4
##### 5
###### 6

```
1
=

2
-
```

1
=

2
-

### Italics

```
*text*
```

*text*

### Bold

```
**text**
```

**text**

```
__text__
```

__text__

### Strikethrough

```
~~text~~
```

~~text~~

### Links

```
[text](https://www.google.com/)
<a href="https://www.google.com/">text</a>
```

[text](https://www.google.com/)
<a href="https://www.google.com/">text</a>

```
[text](https://www.google.com/ "tooltip")
<a href="https://www.google.com/" title="tooltip">text</a>
```

[text](https://www.google.com/ "tooltip")
<a href="https://www.google.com/" title="tooltip">text</a>

```
[text](#links)
```

[text](#links)

### Code

```
non-code `inline-code`
```

non-code `inline-code`

~~~
```
multi-line
code
```

    alternatively,
    indent with 4 spaces
~~~

```
multi-line
code
```

    alternatively,
    indent with 4 spaces

~~~
```c
// syntax-highlighted
int main()
{
	printf("multi-line code");
}
```
~~~

```c
// syntax-highlighted
int main()
{
	printf("multi-line code");
}
```

### Quotes

```
> text
```

> text

```
> multi-line <br>
> quote
> > nested quote
```

> multi-line <br>
> quote
> > nested quote

### Tables

```
Cat 1 | Cat 2 | Cat 3 | Cat 4
----- | ----- |:-----:| -----:
text | text | text | text
more text | more text | centered text | right-aligned text
 | | | | 
```

Cat 1 | Cat 2 | Cat 3 | Cat 4
----- | ----- |:-----:| -----:
text | text | text | text
more text | more text | centered text | right-aligned text
 | | | | 

### Lists
 
```
* text
* text
  * text
    * text
      * text
```

* text
* text
  * text
    * text
      * text

```
1. text
2. text
   1. text
      1. text
         1. text
```

1. text
2. text
   1. text
      1. text
         1. text
		 
```
- [ ] text
- [X] text
  - [X] text
    - [X] text
- [X] text
  * text
    * text
  1. text
     1. text
```

- [ ] text
- [X] text
  - [X] text
    - [X] text
- [X] text
  * text
    * text
  1. text
     1. text
	 
### Images

```
![alt text](https://github.com/JarateKing/Github-Markdown-Snippets/blob/master/dev/example.png)
![alt text](dev/example.png)
```

![alt text](https://github.com/JarateKing/Github-Markdown-Snippets/blob/master/dev/example.png)
![alt text](dev/example.png)

## HTML

Github flavored markdown supports HTML tags and attributes, and is useful for advanced techniques within markdown. There's a whitelist of supported tags and attributes however, and the HTML that is usable is very restrictive.

### Tags

The code for the whitelisted tags can be found [here](https://github.com/jch/html-pipeline/blob/master/lib/html/pipeline/sanitization_filter.rb#L42)

```h1 h2 h3 h4 h5 h6 h7 h8 br b i strong em a pre code img tt
div ins del sup sub p ol ul table thead tbody tfoot blockquote
dl dt dd kbd q samp var hr ruby rt rp li tr td th s strike summary
details caption figure figcaption
abbr bdo cite dfn mark small span time wbr
```

### Attributes

The code for the whitelisted attributes can be found [here](https://github.com/jch/html-pipeline/blob/master/lib/html/pipeline/sanitization_filter.rb#L57)

```
abbr accept accept-charset
accesskey action align alt
aria-describedby aria-hidden aria-label aria-labelledby
axis border cellpadding cellspacing char
charoff charset checked
clear cols colspan color
compact coords datetime dir
disabled enctype for frame
headers height hreflang
hspace ismap label lang
maxlength media method
multiple name nohref noshade
nowrap open prompt readonly rel rev
rows rowspan rules scope
selected shape size span
start summary tabindex target
title type usemap valign value
vspace width itemprop
```

### Entities

A list of named html entities can be found [here](https://en.wikipedia.org/wiki/List_of_XML_and_HTML_character_entity_references#Character_entity_references_in_HTML)

Some common ones:

Code | Appearance
---- | ----------
`&copy;` | &copy;
`&reg;` | &reg;
`&para;` | &para;
`&micro;` | &micro;
`&times;` | &times;
`&divide;` | &divide;
`&deg;` | &deg;
`&plusmn;` | &plusmn;

Html entities can be referenced by their unicode number. For example, `&copy;` is equivalent to `&#xa9;` (for hexadecimal) or `&#169;` (for decimal).

### Emojis

A list of valid emoji shortcodes can be found [here](Emoji-list.md)

```
:shark:
```

:shark:

## Text

### Subscripts

`text<sub>subscript</sub>`

text<sub>subscript</sub>

### Superscripts

`text<sup>superscript</sup>`

text<sup>superscript</sup>

## Alignments

### Center Aligned

`<p align="center">text</p>`

<p align="center">text</p>

### Right Aligned

`<p align="right">text</p>`

<p align="right">text</p>

### Split Page

```
<table><tbody><tr>
<td width="50%">Left Text</td>
<td width="50%">Right Text</td>
<td></td></tr></tbody></table>
```

<table><tbody><tr>
<td width="50%">Left Text</td>
<td width="50%">Right Text</td>
<td></td></tr></tbody></table>

### Triple Alignment

Note: this only works well for single words, and when the left and right aligned texts are approximately the same length (such as with "prev" and "next", for example). The percents can be fiddled with otherwise, but is less likely to work.

```
<table><tbody><tr>
<td>Left Aligned</td>
<td  width="50%"></td>
<td>Center Aligned</td>
<td  width="50%"></td>
<td>Right Aligned</td>
</tr></tbody></table>
```

<table><tbody><tr>
<td>Left Aligned</td>
<td  width="50%"></td>
<td>Center Aligned</td>
<td  width="50%"></td>
<td>Right Aligned</td>
</tr></tbody></table>

## Images

### Specify Size

```
<img width="10" height="10" src="https://placehold.it/15/ff0000/000000?text=+">
<img width="50" height="50" src="https://placehold.it/15/ff0000/000000?text=+">
```

<img width="10" height="10" src="https://placehold.it/15/ff0000/000000?text=+">
<img width="50" height="50" src="https://placehold.it/15/ff0000/000000?text=+">

## Style

### Surround By Box

```
<table><tbody><tr>
<td>Text to surround box with</td>
</tr></tbody></table>
```

<table><tbody><tr>
<td>Text to surround box with</td>
</tr></tbody></table>

```
<table border="1"><tbody><tr>
<td width="100%">Text to surround box with</td>
<td></td></tr></tbody></table>
```

<table border="1"><tbody><tr>
<td width="100%">Text to surround box with</td>
<td></td></tr></tbody></table>

### Divider Line

```
#
##
```

#
##

```
---
***
___
<hr>
```

---
***
___
<hr>

```
<img width="100%" height="3" src="https://placehold.it/15/eeeeee/000000?text=+">
```

<img width="100%" height="3" src="https://placehold.it/15/eeeeee/000000?text=+">

### Hotkey Styling

```
<kbd>Text</kbd>
```

<kbd>Text</kbd>

### Dropdown / Collapsing / Spoilers

```
<details><summary>Click</summary>
Text</details>
```

<details><summary>Click</summary>
Text</details>

```
<details><summary>Click</summary>
  
* Text
* Text
* Text</details>
```

<details><summary>Click</summary>
  
* Text
* Text
* Text</details>

### Start-of-line Asterisk

Normally, having an asterisk at the start of a line will become a list. If you want to keep it as an asterisk, you can add a zero-width whitespace character in front of it. This same logic will also apply to other markdown concepts.

```
* Text
```

* Text

```
&#8203;* Text
```

&#8203;* Text

## Composed

### Table of Contents

```
<table><tbody><tr>
<td><details><summary>Table of Contents</summary>

1. [Category 1](#html)
   1. [Subcategory 1](#tags)
   2. [Subcategory 2](#attributes)
2. [Category 2](#text)
3. [Category 3](#alignments)
</details></td>
</tr></tbody></table>
```

<table><tbody><tr>
<td><details><summary>Table of Contents</summary>

1. [Category 1](#html)
   1. [Subcategory 1](#tags)
   2. [Subcategory 2](#attributes)
2. [Category 2](#text)
3. [Category 3](#alignments)
</details></td>
</tr></tbody></table>

### Captioned Image

```
<table><tbody><tr>
<td>
	
<p align="center">
<img src="https://github.com/JarateKing/Github-Markdown-Snippets/blob/master/dev/example.png">
</p>

<p align="center"><sub>Example Caption Here</sub></p>
</td>
</tr></tbody></table>
```

<table><tbody><tr>
<td>
	
<p align="center">
<img src="https://github.com/JarateKing/Github-Markdown-Snippets/blob/master/dev/example.png">
</p>

<p align="center"><sub>Example Caption Here</sub></p>
</td>
</tr></tbody></table>