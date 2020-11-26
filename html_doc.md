# Doctype
It defines the type of document which we are going to use. There some other doctype like :- **math ML**, **SVG** etc.
### Syntax
```html
<!DOCTYPE html>

<!DOCTYPE math PUBLIC "-//W3C//DTD MathML 2.0//EN"	
    "http://www.w3.org/Math/DTD/mathml2/mathml2.dtd">
    
<!DOCTYPE svg:svg PUBLIC
    "-//W3C//DTD XHTML 1.1 plus MathML 2.0 plus SVG 1.1//EN"
    "http://www.w3.org/2002/04/xhtml-math-svg/xhtml-math-svg.dtd">
```

Why it is important ?

> If someone other than your team works on the same project then they will get to know that what **type** of doc it is and which **version**.

> If browser sees this then they compile your whole doc according to that. If you don't write the type of doc it is then browser have to predict by its own again n again.

# Elements and Attribute

**Elements** : Whatever you sees all are elements, like _paragraph,link,image,video_ etc.
```
    <TagName>Content</TagName>
```
**Example:** `<p>This is paragraph tag</p>`

**Attribute** : Additional info about elements
```
    <TagName attribute1="value1" attribute2="value2">Content</TagName>
```
**Example:** `<p width="100px">This is paragraph tag</p>`

**NOTE:** There is some empty html tag, which means they don't have closing braces. **i.e** `<img>, <br>` etc.

# Indentation
```
    This makes code clean and readable.
```

# HTML Comments
```
    Comments is very useful in debugging html code and understanding code for the changes.
```

# Headings
It is very useful in SEO. It increases the google ranking.

`<h1>Heading 1</h1>` <br>
`<h2>Heading 2</h2>` <br>
`<h3>Heading 3</h3>` <br>
`<h4>Heading 4</h4>` <br>
`<h5>Heading 5</h5>` <br>
`<h6>Heading 6</h6>` 

# Paragraph
* Paragraph tag removes **Extra Space** and **Line Break** by its own.
* To use that extra spaces and line break you have to use tag `<pre>content</pre>`, this tag will show your paragraph as it is.This is is used very least.
* Second alternative is to use `<p>content</p>` with some other tags which will satisfy our end result. Tags are `<br>`
* There are some tags which is used to manipulate paragraph such as

    `<b></b>` <br>
    `<strong></strong>` -> same as bold tag.very effective in SEO.don't over use other wise google will understand that you are forcing. <br>
    `<i></i>` <br>
    `<em></em>` -> same as i tag. good for SEO. perfect for screen reader. <br>
    `<small></small>` <br>
    `<mark></mark>` <br> -> This will highlight the text.
    `<del></del>` <br>
    `<ins></ins>` <br>
    `<sub></sub>` -> x<sub>3</sub> <br>
    `<sup></sup>` -> y<sup>2</sup>
 
# Formatting
# Quotation and citation

`<q></q>` -> This will just add double quote to the content i.e "hey i am you tutor" <br>
`<blockquote cite="https://google.com"></blockquote>` -> This will take spaces from all side.Cite says that from where you have took this article. <br>
`<abbr></abbr>` -> This will tell full form of word on hover. <br>
`<address></address>` -> This tag will help in SEO.

# HTML Links
* This will be used in navigation from one page to another page.

`<p id="first">content............<p>` <br>
`<a href="#first" target="_blank" title="Goto upper section">Read More</a>` -> Here **id** in **href** will be used for navigation. **target** is used to open in new tab. **title** used for showing hint on hovering link. <br>

# Email Links
* This is very useful in contact us section. Whenever user click on this link the email application on their respective device will open and the email will directly comes into **TO** section. We can also add **subject**.

```
<p>
    <h3>Contact Us</h3> <br>
    <a href="mailto:admin@website.com?subject=Tech Support">admin@website.com</a>
</p>
```
# Images
* This is an empty tag. <br>
    `<img src="/images/girl_1.jpg" alt="Beautiful girl" width="500px" height="500px">` <br>
    **alt** will be used when your image will broke and it is also good for screen reading.
# Marquee
* Now this is depricated from html 5 but browser does support this. <br>
    `<marquee behavior="" direction="right"> This is moving text</marquee>`

# Ordered List
```
<ol start="" type="i">
    <li>Coffee</li>
        <ol type="a">
            <li>Mocha</li>
            <li>Laatee</li>
        </ol>
    <li>Tea</li>
    <li>Milk</li>
</ol>
```    
# Unordered List
```
<ul style="list-style-type: circle;">
    <li>Coffee</li>
        <ul style="list-style-type: square; 
        list-style-position: inside; background-color: chartreuse;">
            <li style="border: 1px solid red;">Mocha</li>
            <li>Laatee</li>
        </ul>
    <li>Tea</li>
    <li>Milk</li>
</ul>
```
# Description List
# HTML Table
# Nested Table
# Div and Span
* Div is a block element
    - Always takes full width.
    - Always starts with new line.
    - We can set height and width to this.

![Block Elements](images\doc_img\block_element.png)

* Span is a inline element
    - It always take space according to the content.
    - I didn't starts with new line.
    - We can not set height and width to this.

![Block Elements](images\doc_img\span_tag.png)

* List of inline elements

![Block Elements](images\doc_img\inline_elements.png)
# Iframe
* It is used to show other's website into your websites.
* Some websites are restricted to this so you can't show that websites to your website.
* Use case
    - If you want to compare two news channel covid tally for example.

* Syntax

    `<iframe src="https://www.ndtv.com/" frameborder="0" height="500" width="500"></iframe>`
# HTML Audio
* This is used to show some audio to the user on your website

```
<audio controls>
    <source src="audio\Tujhe Kitna Chahne Lage - Kabir Singh.mp3" type="audio/mpeg">
    <source src="audio\Tujhe Kitna Chahne Lage - Kabir Singh.ogg" type="audio/ogg">
    Your browser does not support audio file
</audio>
```

# HTML Video

# Embed PDF
# Embed Youtube Video
# Embed Google Maps
# HTML Entities
# HTML Symbols
# Emojis in HTML
# Semantic Elements
# HTML Image Maps
# HTML Forms
# Form Input Types
# Form File Upload
# HTML Input Attribute
# HTML Textarea and image button
# Select Option
# Radio Button
# Checkbox
# DataList
# Label, Fieldset and legends
# SEO Tags
# Favicon
# Style in head Tag
# Script and no script
# Open Graph and Twitter card Tag
# Viewport Meta TAg
# Right to Left Website
# W3c HTML Validation