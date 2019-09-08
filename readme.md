# A husband's guide to HTML

## Paragraphs

First thing's first, to create a paragraph of text, simply wrap your text in a `<p>` tag, and then close your paragraph with `</p>`. You can copy and paste the below code to make a paragraph.

``` html
<p>This ia paragraph of text.</p>

<p>This is another paragraph.</p>
```

### Line breaks

Adding a line break to your text is as simple as using the below HTML:

```html
<br/>
```

## Headlines

In HTML we can create headlines for sections using the below markup:

```html
<h1>Headline 1</h1>
<h2>Headline 2</h2>
<h3>Headline 3</h3>
<h4>Headline 4</h4>
<h5>Headline 5</h5>
<h6>Headline 6</h6>
```

# Headline 1
## Headline 2
### Headline 3
#### Headline 4
##### Headline 5
###### Headline 6

As you can see, the largest headlines start at 1 and go down to 6. In general, Headline 1 should only be used **once** per page, and generally should be the description of the page, or the most important headline on the page. Headline 2 should be preferred for sections, followed by 3, then 4, and so on. It's rare to use anything past Headline 3, but it happens.


## Lists

Lists can be 'undordered lits' or 'ordered lists'. The difference is 'ordered lists' list their items numerically, generally.

An ordered list looks like this:

1. First list item
2. Second list item
3. Third list item

You can copy and paste this code to make an ordered list:

```html
    <ol>
        <li>First list item</li>
        <li>Second list item</li>
        <li>Third list item</li>
    </ol>
```

An unordered list looks like this:

* First unordered list item
* Second unordered list item
* Third unordered list item

Copy and paste this code to make an unordered list:

```html
    <ul>
        <li>First unordered list item</li>
        <li>Second unordered list item</li>
        <li>Third unordered list item</li>
    </ul>
```

## Bold and italic text

To make your text **bold** or _italic_, use the following code:

```html
<strong>bold text</strong>

<em>emphasized, aka italic text</em>
```

## Images

To embed an image, use the below code:

```html
<img src="https://placedog.net/400/225?id=12" alt="Corgi on the beach">
```

![Corgi on the beach](https://placedog.net/400/225?id=12 "Corgi on the beach")

Note that the `src` points to where the image is on the server and `alt` describes the image. It's best practice to add some sort of alternative text, and to keep it fairly general unless specification is necessary. If an image is purely decorative, alt-text is not required, however it's preferable to have it.

## Links

To link from your text to another place online, you'll want to wrap it in `<a>` tag markup. You'll want to use the below code:

```html
<!--Opens link in the same tab/window-->
<a href="https://google.com">Link 1</a>

<!--Opens link in a new tab/window-->
<a href="https://google.com" target="_blank">Link 2</a>
```

Note, as the commented code above the link says, that to open your link in a new tab or new window, simply add the `target="_blank"` attribute to your link markup. You can also use `target="_self"` to open your link in the same window, but the default browser behaviour does not require it.

## Styles

While you generally want to style your text with a Cascading Style Sheet, aka CSS, in cases where a stylesheet is not accessible, you can style your text, or anything really, with 'inline styles'.

**It's not best practice, but it works.**

An example of an inline style, say changing the color of text, can be done like so:

```html
<p style="color:coral">This is coral colored text.</p>
```

Notice that in this instance, we're asking the browser to use the `coral` color, rather than using Hex code. Hex code generally looks like this: `#f88379` (coral in HEX). You'll want to use Hex code generally, a handy guide to find the color you want can be found here online at [https://htmlcolorcodes.com/color-picker/](https://htmlcolorcodes.com/color-picker/)

Anything doable with CSS can be done with inline styles. You can even add multiple styles, for instance to make our text red and a bigger font size, you can do the below:

```html
<p style="color:coral;font-size:18px;">This is some red text at 18px.</p>
```

Note that the `;` is added to the end of each style. Ideally, you should not need to use the `font-size` style attribute since there are other options available to add larger text.  
