# HTML and CSS

# HTML and CSS

HTML (Hypertext Markup Language) and CSS (Cascading Style Sheets) are two essential web development technologies used to create visually appealing and interactive web pages. HTML provides the structure and content of a website while CSS controls the presentation and style.

HTML is a markup language used to create web pages. It uses various tags and attributes to define the content of a web page such as headings, paragraphs, images, links, and more. HTML tags provide a way to structure and organize content on a webpage.

![Screenshot 2023-05-19 222739.png](HTML%20and%20CSS%20b2d52bbdbcac4726b5042b204f17f0a2/Screenshot_2023-05-19_222739.png)

## HTML basic tags

- <html></html>  - Surround entire document
- <head></head>- Surround header material (titles, css info,
etc.
- <body></body> - Contains the main content of the page
- <p></p> - Hold a single paragraph that the browser will
typeset.
- <img> - Will display an image
   * mage file must be in a popular graphics format (gif, jpg, png, etc)
- <ul></ul> Unordered List
- <ol></ol> Ordered List
- <li></li> Encloses a single list item

HTML – Example: Lists

```html
HTML – Example: Lists
<!DOCTYPE html>
<html>
<body>
<h2>Unordered List</h2>
<ul>
<li>Coffee</li>
<li>Tea</li>
<li>Milk</li>
</ul>
<h2>Ordered List</h2>
<ol>
<li>Coffee</li>
<li>Tea</li>
<li>Milk</li>
</ol>
</body>
```

- Coffee
- Tea
- Milk

## Ordered List

1. Coffee
2. Tea
3. Milk

- <b></b> - Bold text
- <strong></strong> - Important text (similar to bold
- <i><i> - Italic text
- <em></em> - Emphasized text (similar to Italic)
- <mark></mark> - Marked text
- <small><small> - Small text
- <del></del> - Deleted text (stroked text)
- <ins></ins> - Inserted text
- <sub></sub> - Subscript text
- <sup></sup> - Superscript text and so on..,

# CSS

CSS is a style sheet language used to describe the presentation of a web page. It can be used to define the layout, colors, fonts, and other design elements of a webpage. CSS works by associating style rules with HTML elements.

CSS = Cascading Style Sheets
Greatly simplifies styling HTML

Easy to keep consistent styling

Instructions are written as a rule-set

### CSS rule-sets

CSS rule-sets have the following format:

![Screenshot 2023-05-19 224819.png](HTML%20and%20CSS%20b2d52bbdbcac4726b5042b204f17f0a2/Screenshot_2023-05-19_224819.png)

- Selectors indicate the tag or other element
- Property/value pairs give the attribute to define and the value of the attribute
- Property/value pairs are separated with a semicolon ;

## CSS - Selectors

Selectors can be
• A tag name (i.e. <p>) —This will apply to all tags of that type in the document
• An id (<h2 id="foo">) —The style will apply to ANY tag with the named id.

• A class (<p class="LargeRed">) The style will apply to ANY element with the named class)

### CSS – Examples: Selectors

![Screenshot 2023-05-19 225256.png](HTML%20and%20CSS%20b2d52bbdbcac4726b5042b204f17f0a2/Screenshot_2023-05-19_225256.png)

### CSS - Borders

  
CSS allows specification of the style, width and color of element
borders
• Attributes:
       • **border-style** : style keyword — includes dotted, dashed, solid, double, groove, ridge, inset,                 outset, none, hidden}

    • **border-width** : Value can be specified in pt, px, cm, em ; Value can use one of 3 keywords: thin, medium, thick

In conclusion, HTML and CSS are essential web development technologies that work together to create visually appealing and interactive web pages. Developers use these technologies to create responsive and optimized web pages that provide an excellent user experience.

### Summary

**HTML** — Hyper Text Markup Language used to describe most web page content Static — no 'execution' semantics.
**CSS** — Cascading Style Sheets; Help customize look and feel of web pages; Numerous ways to address elements and groups of elements; Varied properties to produce rich styling.