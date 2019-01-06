# Github Markdown Snippets

# HTML

Github flavored markdown supports HTML tags and attributes, and is useful for advanced techniques within markdown. There's a whitelist of supported tags and attributes however, and the HTML that is usable is very restrictive.

## Tags

The code for the whitelisted tags can be found [here](https://github.com/jch/html-pipeline/blob/master/lib/html/pipeline/sanitization_filter.rb#L42)

```h1 h2 h3 h4 h5 h6 h7 h8 br b i strong em a pre code img tt
div ins del sup sub p ol ul table thead tbody tfoot blockquote
dl dt dd kbd q samp var hr ruby rt rp li tr td th s strike summary
details caption figure figcaption
abbr bdo cite dfn mark small span time wbr
```

## Attributes

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

# Text

## Subscripts

`text<sub>subscript</sub>`

text<sub>subscript</sub>

## Superscripts

`text<sup>superscript</sup>`

text<sup>superscript</sup>

# Alignments

## Center Aligned

`<p align="center">text</p>`

<p align="center">text</p>

## Right Aligned

`<p align="right">text</p>`

<p align="right">text</p>

## Split Page

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

## Triple Alignment

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
