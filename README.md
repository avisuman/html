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
* Second alternative is to use `<p>content</p>` with some other tags which will satisfy our end result. Tags are `<br>,&nbsp;`
* There are some tags which is used to manipulate paragraph such as

    `<b></b>` <br>
    `<strong></strong>` -> same as bold tag.very effective in SEO.don't over use other wise google will understand that you are forcing. <br>
    `<i></i>` <br>
    `<em></em>` -> same as i tag. good for SEO. perfect for screen reader. <br>
    `<small></small>` <br>
    `<mark></mark>` -> This will highlight the text. <br>
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
* This is used to embed video on webpage
```
<video controls >
    <source src="./video/videoplayback.mp4" type="video/mp4">
    <source src="./video/videoplayback.ogg" type="video/ogg">
    Your browser does not support video.
</video>
```

# Embed PDF
* There are three way to embed pdf on web page
    - embed tag <br>
        - Type is important here <br>
            `<embed src="./pdf/Git-Cheat-Sheet.pdf" type="application/pdf" width="1000" height="500">`
    - iframe <br>
        - Type is not required here <br>
            `<iframe src="./pdf/Git-Cheat-Sheet.pdf" frameborder="0" width="800" height="800"></iframe>`
    - object
        - Type is important here <br>
            `<object data="./pdf/Git-Cheat-Sheet.pdf" type="application/pdf" width="1200" height="500"></object>`
# Embed Youtube Video
* You can only embed those youtube videos which are open/allowed.
* Just open youtube and then video which you want to embed then click on share button copy the code and simply paste to your html file. <br>
```
<iframe width="560" height="315" src="https://www.youtube.com/embed/5UT0_uS27SI" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```    
# Embed Google Maps
* To embed google map to your webpage just open the desired location and click on share and then click on embed a map. copy the html code and just paste to html file.
```
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3680.263078102819!2d75.8525280142765!3d22.71846113332779!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3962fd0a3c2422a1%3A0xb8cf3a1b62708158!2sRajwada%20Palace!5e0!3m2!1sen!2sin!4v1606371831166!5m2!1sen!2sin" width="600" height="450" frameborder="0" style="border:0;" allowfullscreen="" aria-hidden="false" tabindex="0"></iframe>
```
# HTML Entities
* This is used to print reserve character of html.
* We can write this by using two methods : <br>
    - By using **name** <br>
        - Syntax : `&name;`
        - Example: Write `<div>` tag <br>
                    `&lt;div&gt;`
    - By using **number** <br>
        - Syntax : `&#number;`
        - Example: Write `<div>` tag <br>
                    `&#60;div&#62;`

* Note: One important which is used for extra spaces between characters in paragraph. i.e **nbsp** <br>
    - Example: `<p>Hello &nbsp; &nbsp; &nbsp; world</p>`

# HTML Symbols
* This is very useful when you have to show symbol of currency, copyright etc <br>
    - Example : `&copy;` or `&#8508;`

# Emojis in HTML
* This is also symbol but have some special meaning which resemble to human behaviour. <br>
    - Example : `&#128516`
    - You can find emojis code number from here <br>
    [w3schools Emojis](https://www.w3schools.com/charsets/ref_emoji.asp)

# Semantic Elements
* Semantic Elements = elements with a meaning.
* A semantic element clearly describes its meaning to both the browser and the developer.
* Examples of **non-semantic** elements
    - `<div>` and `<span>` - Tells nothing about its content.
* Examples of **semantic** elements
    - `<form>`,`<table>`,`<article>` - Clearly defines its content. <br> <br>

**Old Non Semantic Element**
![Old Non Semantic Element](images\doc_img\semantic.png) <br><br>
**New Semantic Element in HTML5**
![New Semantic Element in HTML5](images\doc_img\new_html5_semantic.png) <br><br>
**Difference between HTML 4 and HTML 5**
![diff between html4 and html5](images\doc_img\html4-html5.png) <br><br>
**Difference between HTML 4 and HTML 5 code**
![diff between html4 and html5 code](images\doc_img\code-diff.png)

# HTML Image Maps
* This is very useful when you have to add multiple links to single image. <br>
**We will write code for below image** <br><br>
![banner](images\banner.jpg) <br><br>
```
<img src="./images/banner.jpg" alt="Banner" usemap="#banner">
<map name="banner">
    <area shape="rect" coords="305,43,567,229" href="https://thenatures.in/product-category/regular-grocery/foodgrains/" alt="Hot Spot">
    <area shape="poly" coords="595,175 611,106 664,50 716,50 737,73 776,67 797,83 808,99 822,119 845,119 866,124 874,128 882,140 865,154 852,154 840,172 840,191 840,218 822,229 790,245 767,241 757,241 741,252 718,262 684,250 672,236 649,221 625,198 602,179" href="https://thenatures.in/product-category/regular-grocery/biscuits-snacks-namkeen-chips/" alt="Hot Spot">
    <area shape="poly" coords="1044,12 1090,55 1098,97 1114,140 1139,159 1122,269 1113,276 943,276 937,252 955,206 966,151 976,138 994,108 992,92 997,85 1010,37 1017,30 1040,12 " href="https://thenatures.in/product-category/personal-care/" alt="Hot Spot">
</map>
```

# HTML Forms
* Form is used for collecting data from user
```
<form action="submit.php" method="POST">
    <div>
        Name: <input type="text">
    </div>
    <div>
        <br>
        <input type="button" value="Submit">
    </div>
</form>
```
* Attribute **action** tells that, take the filled data by user to given file.
* Attribute **method** this will specify how your data will be transferred.

# Form Input Types
* There are many input types which are listed below <br>

```
<form action="">
    <div>
        Text: <input type="text"> <br>
    </div>
    <div>
        Submit Button: 
        <input type="button" value="Submit">
    </div>
    <div>
        Colour:
        <input type="color"> <br>
    </div>
    <div>
        Date:
        <input type="date"> <br>
    </div>
    <div>
        Email:
        <input type="email"> <br>
    </div>
    <div>
        Hidden:
        <input type="hidden" value="Indore"> <br>
    </div>
    <div>
        Number:
        <input type="number"> <br>
    </div>
    <div>
        Password:
        <input type="password"> <br>
    </div>
    <div>
        Reset:
        <input type="reset">
    </div>
    <div>
        Time:
        <input type="time">
    </div>
    <div>
        URL:
        <input type="url">
    </div>
    <div>
        Range:
        <input type="range" min="1000" max="5000">
    </div>
</form>
```    
# Form File Upload
* This is used to provide the file uploading functionality to user
    - In below example **type** gives functionality of uploading files.
    - By using **multiple** we can upload multiple files.
    - **enctype** is used because sometimes data is very big, in this scenario it is not advisable to sent data at once. So we have to send this as multipart.

```
<form enctype="multipart/form-data">
    <input type="file" multiple>
</form>
```

# HTML Input Attribute
* Attribute used for modifying the input tag. Some of them are listed below: <br>
    - **value** is used for visual information. i.e `<input type="submit" value="Submit">`
    - **readonly** is used for restricting user from editing the value. i.e `<input type="text" value="Avinash" readonly>`
    - **disabled** will be shown as fadded field. i.e `<input type="text" value="Avinash" disabled>`
    - **size** will show the no of character at a time. i.e `<input type="text" value="Avinash" size="50">`. Here only 50 character will be shown after that all be invisible.
    - **maxlength** will restrict user to enter the character of given length. i.e `<input type="number" value="9713933556" maxlength="10" size="50">`
        - maxlength is mainly used in **number, range, and date** <br>
            - `<input type="number" value="" max="10" min="10" size="50">`
    - **placeholder** is used for hint. i.e `<input type="text" value="" placeholder="Enter your full name">`
    - **required** is used for making any field required/compulsory.
    - **step** is used for increasing number in multiple of 5. i.e `<input type="number" value="1" step="5">` 
    - **autofocus** bring direct focus and curser there to start writing. i.e `<input type="text" value="" placeholder="Enter your full name" autofocus>`
    - **name** is used for backend purpose i.e by what name data will be received there.

# HTML Textarea and image button
* **Textarea** is used for taking long feedback, descriptions etc. <br>
    - `<textarea name="input-text" id="text-id" cols="30" rows="10"></textarea>` 

* **Image Button** 
    - `<input type="image" value="iamge-button" src="/images/banner.jpg" width="100" height="50">`
# Select Option
```
<form action="">
    <select name="" id="" size="5" multiple>
        <option value="">Audi</option>
        <option value="">BMW</option>
        <option value="" selected>Tata</option>
        <option value="">Honda</option>
        <option value="">Maruti</option>
        <option value="">Hero</option>
    </select>
</form>      
```
```
<form action="">
<select name="" id="">
    <optgroup label="Cars"> 
        <option value="">Audi</option>
        <option value="">BMW</option>
        <option value="" selected>Tata</option>
        <option value="">Honda</option>
        <option value="">Maruti</option>
    </optgroup>
    <optgroup label="Luxary Cars">
        <option value="">Hero</option>
        <option value="">Hundai</option>
        <option value="">Datsun</option>
        <option value="">Jeep</option>
        <option value="">Kia</option>
    </optgroup>
    <optgroup label="Sports">
        <option value="">Cricket</option>
        <option value="">Football</option>
        <option value="">Kabbadi</option>
        <option value="">Basketball</option>
        <option value="">Carram</option>
        <option value="">Chess</option>
    </optgroup>
    <optgroup label="Actors">
        <option value="">Akshay</option>
        <option value="">Sunny Deol</option>
        <option value="">Divya Bharti</option>
    </optgroup>
</select>
</form>
```

# Radio Button
```
<form action="">
    <input type="radio" name="gender" value="male"> Male
    <input type="radio" name="gender" value="female" checked> Female
    <input type="radio" name="gender" value="other"> Other
    <br><br>
    <input type="radio" name="emptype" value="other"> Permanent
    <input type="radio" name="emptype" value="other" checked> Temporary
</form>
```
# Checkbox
* This is used to receive multiple value in only one variable.
```
<form action="">
    <input type="checkbox" name="sports" value="other"> cricket
    <input type="checkbox" name="sports" value="other" checked> Football
</form>
```
# DataList
```
<form action="">
    Search <input type="text" list="search-prediction" autofocus>
    <datalist id="search-prediction">
        <option value="Apple">
        <option value="Ball">
        <option value="Mango">
        <option value="Car">
        <option value="Mobile">
        <option value="Laptop">
    </datalist>
</form>
```

# Label, Fieldset and legends
* Label is good for search engine, screen reader and user
```
<form action="">
    <div>
        <label for="fname">First Name</label>
        <input type="text" id="fname">
    </div>
    <div>
        <input type="submit">
    </div>
</form>
```
* Fieldset is used for grouping withing form
```
<form action="">
    <fieldset>
        <legend>Basic Information</legend>
        <label for="fname">First Name</label>
        <input type="text" id="fname">
        <label for="lname">Last Name</label>
        <input type="text" id="lname">
    </fieldset>
    <fieldset>
        <legend>Other Information</legend>
        <label for="address">Address</label>
        <input type="text" id="address">
        <label for="mobile">Mobile</label>
        <input type="text" id="mobile">
    </fieldset>
    <div>
        <input type="submit">
    </div>
</form>
```
# SEO Tags
```
<head>
    <title>Tech Gun Html</title>
    <meta name="description" content="This is a page about car" />
    <link rel="canonical" href="car.html" />
    <meta name="robots" content="index, no follow" />
</head>
```

# Favicon
* This can created though online website too. 
    - `<link rel="shortcut icon" href="./images/girl_1.jpg" type="image/x-icon">`
    ![Favicon Generation Online](https://realfavicongenerator.net/)

# Style in head Tag
# Script and no script
# Open Graph and Twitter card Tag
# Viewport Meta TAg
# Right to Left Website
# W3c HTML Validation
