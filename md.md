<link rel="preload" as='style' href="https://actwu.github.io/md2.css"/>
<link rel="stylesheet" href="https://actwu.github.io/md2.css"/>
<script src="https://cdn.jsdelivr.net/gh/iselang/iselang.github.io@main/num.min.js"></script>


My favorite theme / ui i use in md
For pure MD

```html
<link rel="preload" as='style' href="https://actwu.github.io/md2.css"/>
<link rel="stylesheet" href="https://actwu.github.io/md2.css"/>
<link rel="preload" href="https://cdn.jsdelivr.net/gh/iselang/iselang.github.io@main/num.min.js"/>

<script src="https://cdn.jsdelivr.net/gh/iselang/iselang.github.io@main/num.min.js"></script>
<script>
app('Im lazy'); fav(2);
</script>
```

For Html using MDE
```html
<link rel="preload" href="https://actwu.github.io/mde/l.js">
<link rel="preload" href="https://cdn.jsdelivr.net/gh/iselang/iselang.github.io@main/num.min.js"/>
<link rel="preload" href="https://cdn.jsdelivr.net/gh/iselang/iselang.github.io@main/num.min.js"/>

<md>

</md>

<script src="https://actwu.github.io/mde/l.js"></script>
<script src="https://cdn.jsdelivr.net/gh/iselang/iselang.github.io@main/num.min.js"></script>
<script>
app('Im lazy'); fav(2);
</script>


```

# Markdown Language (Md)
- A Text media used in making notes or text...
  This is commonly used in making design text in a easy way.


Basically html but simple.
Mainly used in documentations.

It is also rendered as html,
That's why you could put html codes

## Syntax

## Text
```markdown
This is a text no need to write codes
for a text
```
## Make text **Bold**
Put 2 of asterisk sign (*) from start and ending
```markdown
**this Is a bold text**
```
Output
>
> **this Is a bold text**
>

## Make text ***Bold Italic***
Put 3 of asterisk sign (*) from start and ending
```markdown
***this Is a italic text***
```
Output
> 
> ***this Is a bold italic text***
>

## Make text *Italic*
Put 3 of asterisk sign (*) from start and ending
```markdown
*this Is a italic text*
```
Output
> 
> *this Is a bold italic text*

## Make text Text Block

```markdown
> this Is a text block
```
Output
> 
> this Is a text block
>

## Code Block
```markdown

` ` ` t y p e
t h i s  i s  w h e r e  y o u  p u t  t h e  c o d e s
` ` `
```

<script>
app('Learn-MD'); fav(2);
</script>

## Button
```markdown
[Button Name](/file)
```
