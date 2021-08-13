![Image of for guide](https://source.unsplash.com/dGqWUPPesrQ)

### About

- This is just a short guide to how you should use typography in your web design and leverage the power of typography in your css.

### A Guide Into How to Use Typography in CSS

1. If no css is defined for font-family, then the font-family will default to your browser and OS' deafult settings for fonts. The OS settings can be different depending on which OS you are using.

Here are the default settings for MacOS and Windows:

- Windows: Arial, Lucida, Impact, Times New Roman, Courier New, Tahoma, Comic Sans, Verdana, Georgia, Garamond

- Mac: Helvetica, Futura, Bodoni, Times, Palatino, Courier, Gill Sans, Geneva, Baskerville, Andale Mono

```
Pro tip: It's a good idea to include these font styles in your font-family settings as you know that the user will definitely be able to see this style of fonts as it is definitely installed on their operating system.
```

2. How does css fonts work with the browser and your OS? The browser will check what font-famliy you have defined in your css in your web app and find one of those font styles on your OS to display the text to you.

For example, if you have the following in your css style sheet. The system will look for Verdana first, then Geneva and so on and so on.

```
font-family: Verdana, Geneva, Arial, Helvetica, sans-serif;
```

Here are some generic font styles:

- serif
- sans-serif
- monospace
- cursive
- fantasy

3. As you saw above, font-family property in css is a prioritized list of font family names. The first font style listed has the highest priority.

4. If you want to use the native font of the operating system, you can use something like this:

```
.some-element {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen-Sans, Ubuntu, Cantarell, "Helvetica Neue", Helvetica, Arial, sans-serif;
}
```

5. Lets look at some of the generic css font styles in more detail.

```
Pro tip: Sans-serif and serif are keywords and should not be put in quotes. Any generic font family names MUSt not be put in quotes.
```

So this would be wrong:

```
font-family: Helvetica "serif"
```

- Sans-serif is French for “without serif”. These are fonts without the decorative small line at the end of their letter/symbol strokes.
- serif: The most common serif font is ‘Times Roman’. I’m pretty sure you’ve seen it around.
- Sans-serif: The most common typeface in this category is Helvetica.
- A monospaced font is also called a fixed-width font. The widths of the characters are fixed!
- Best use: In standard body texts, they aren’t very good. They are harder to read and take up more horizontal space. In the dev world, they are famously used for code blocks
- Cursive fonts are also called script fonts. They are representational of handwriting - this isn’t always the case though.
- Fantasy fonts are primarily decorative fonts that contain playful representations of characters. Sounds like fun, huh?

```
Pro tip: You can use Sans-serif and serif at the end of your font-family list in css as a safety mechanism. As you know that the user will definitely have one of
these font styles installed.
```

Something like this would be good. Here monospace is the safety net. Make sure to enclose font names in quotation marks if they contain spaces.

```
p {
    font-family: "Courier New", "Andale Mono", monospace;
}
```

- In CSS we call the font-family list the font-stack.

6. We will look at "Spacing" next. Usually, when a page does not look right it is due to a spacing problem. So give space to your text both around and within the text.

Something like this is good.

```
body {
    line-height: 1.5;
    padding: 4em 1em;
}
```

7. Next we focus on colors. We do not want sharp black text on sharp white background. This doesn't look too comfortable. Instead, we should use softer colors which make it more comfortable to read.

```
body {
    color: #555;
}
```

We should also have a contrast in colors. So we can do something like this for the headings and subheadings of the text.

```
h1,
h2,
strong {
    color: #333;
}
```
