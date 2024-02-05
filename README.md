# HTML-CSS

HTML &amp; CSS course - January 2024

## Contents

1. [Introduction to HTML & CSS.](#1-introduction-to-html--css)
2. [Typography in CSS.](#2-typography-in-css)
3. [Box Model & Positioning](#3-box-model--positioning)

---

## 1. Introduction to HTML &amp; CSS.

1.  **Introduction to HTML**

    -   _What is HTML?_
        -   This is a markup language.
        -   HTML is the basis for creating web pages and other information that can bedisplayed in a web browser.
        -   Language for expressing semantic structure in textual documents.
        -   HTML is a language for describing web pages.
        -   HTML documents contain HTML tags and plain text.
        -   A markup language is a set of markup tags.
        -   The tags describe document content.
        -   HTML is consumed by web browsers.
        -   The purpose of a web browser is to read HTML documents and compose them intovisible or audible web pages.
        -   The browser does not display the HTML tags, it uses the tags to interpret thecontent of the page.
    -   _HTML Tags:_
        -   Tags are keywords surrounded by angle brackets. - HTML tags normally come inpairs: '<' + 'p' + '>' and '</' + 'p' + '>'
        -   The first tag in a pair is the start tag, the second tag is the end tag.
        -   The end tag is written like the start tag, with a forward slash before thetag name.
        -   Start and end tags are also called opening tags and closing tags.
    -   _Main HTML Tags:_
        -   Describes the start and end of the web page/document - `<html></html>`
        -   Describes the start and end of the metadata section of the document `<head><head>`
        -   Describes the start and end of the web page/document - `<body></body>`
        -   Describes the start and end of the title section of the document - `<title><title>`
    -   _ Example:_
        <img src="https://stuyhsdesign.files.wordpress.com/2015/09/basic-structure.png"width=250 height=150>
    -   _More HTML Tags:_

        -   Headings -
            `<h1> to <h6>`
        -   Paragraphs - `<p>`
        -   Text formating - `<strong>Text</strong>` or `<em>Text</em>`
        -   Links - `<a href="https://softuni.bg">Click this to go to SoftUni.bg</a>`
        -   Images - `<img src="/images/logo.png">`
        -   Ordered List -

                    <ol>
                        <li>List item</li>
                        <li>List item</li>
                    </ol>

        -   Unordered Lst - can be differant types ('disc, circle,square') -

                    <ul
                        <li>list item</li>
                        <li>list item</li>
                    </ul>

        -   Definition List -

                    <dl>
                        <dt>Definition title </dt>
                        <dd>Definition description</dd>
                        <dt>Definition title </dt>
                        <dd>Definition description</dd>
                    </dl>

        -   Table -

                     <table>

                         <thead>
                             <tr>
                                 <th>Table Header 1</th>
                                 <th>Table Header 2</th>
                             </tr>
                         </thead>
                         <tbody>
                             <tr>
                                 <td>Table Cell 1</td>
                                 <td>Table Cell 2</td>
                             </tr>
                         </tbody>

                     </table>

    -   _HTML Tag Attributes:_
        -   Attributes provide additional information about HTML elements
        -   Tags elements can have attributes:
            `<p class='my_theme'>Some text</p>`
        -   Attributes provide additional information about an element
        -   Attributes are always specified in the start tag
        -   Attributes come in name/value pairs like - name="value"
        -   Examples:
            -   _href – gives the tag the location information for the link:_
                `<a href="http://google.bg">Google</a>`
            -   _src – tells the tag where to look for the image file:_
                `<img src="/images/icons/logo.png">`
        -   Some Tips:
            -   Always Quote Attribute Values. Attribute values should always be enclosed in quotes
            -   Double style quotes are the most common, but single style quotes are also allowed
            -   Be careful when combining single and double quotes, make sure you use only one type
            -   Reference Documentation - https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes
    -   _HEAD Tag_ -

        -   The `<head>` element is a container for all the head elements.Elements inside `<head>` can include scripts, instruct the browser where to find style sheets, provide meta information, and more.
        -   The following tags can be added to the head section:
            -   `<title>, <style>, <meta>, <link>, <script>, <noscript>`
        -   Title -

                <head>
                        <title>HTML Document title</title>
                </head>

        -   Link -

                  <head>
                          <link rel="stylesheet" type="text/css" href="style.css">
                  </head>

        -   Meta -

                <head>
                    <!-- Define keywords for search engines: -->
                    <meta name="keywords" content="HTML, CSS, XML, XHTML,JavaScript">
                    <!--Define a description of your web page:-->
                    <meta name="description" content=”Courses on HTML and CSS">
                    <!--Define the author of a page:-->
                    <meta name="author" content=”Koko">
                </head>

2.  Introduction to CSS

    -   _What is CSS?_
        -   CSS stands for Cascading Style Sheets.
        -   Styles define the visual presentation of HTML elements.
        -   CSS solved a problem.
        -   HTML was never intended to contain tags for formatting a document.
        -   With CSS the separation between semantic content and visual presentation can be achieved again.
        -   CSS can save you a lot of work!
        -   External visual style guide shared across all pages of your site.
        -   Change the style guide - change all page's visual presentation.
    -   _CSS syntax:_

        1. Every CSS document is a collection of CSS rules.
        2. CSS rule has two main parts, Select and one or more declarations.
        3. Each declaration consists of a property and a value.

         <img src="https://puzzleweb.ru/en/images/css/1_1.png" width=450px>

        4.  CSS rule has two main parts - SELECTOR and one or more DECLARATIONS!

                [selector]{
                    [declaration]
                    [declaration]
                }

        5.  The CSS Selector is an identifier of the HTML element or the group of HTML elements you want to style.

                body{
                ....
                }

        6.  CSS Declarations end with a semicolon, and declaration groups are surrounded by curly brackets.

                {
                    font:16px/1.5 Verdana, sans-serif;
                    color: #333;
                }

        <img src="https://www.coderepublics.com/CSS/CSS%20Images/css-syntax.webp" width=550px height=150px>

    -   _CSS Selectors_

        -   In CSS, selectors are used to target the HTML elements on our web pages that we want to style
        -   There are a wide variety of CSS selectors available, allowing for fine-grained precision when selecting elements to style
        -   A CSS selector is the first part of a CSS Rule

        1.  _Type selectors_ - The CSS type selector matches elements by node name. In other words, it selects all elements of the given type within a document.

                [tag-name]{                  OR         h1{
                    [declaration]                           color:red;
                    [declaration]                           font-weight:bold;
                }                                       }

        2.  _Class selectors_ - The CSS class selector matches elements based on the contents of their class attribute.

                .[tag-name]{                  OR        .[class-name]{
                    [declaration]                           color:red;
                    [declaration]                           font-weight:bold;
                }                                       }

        3.  _ID selectors_ - The CSS ID selector matches an element based on the value of the element's id attribute. For the element to be selected, its id attribute must match exactly the value given in the selector.

                #[tag-name]{                  OR        #[id-name]{
                    [declaration]                           color:red;
                    [declaration]                           font-weight:bold;
                }                                       }

        4.  _Attribute selector_ - The CSS attribute selector matches elements based on the element having a given attribute explicitly set, with options for defining an attribute value or substring value match.

                [attribute="value"]{          OR        [href="https://google.com"]{
                    [declaration]                           color:red;
                    [declaration]                           font-weight:bold;
                }                                       }

        5.  _Universal selector_ - The CSS universal selector (\*) matches elements of any type.

                *{                            OR        *{
                    [declaration]                           color:red;
                    [declaration]                           font-weight:bold;
                }                                       }

    -   _CSS Combinators_

        1.  _Descendant combinator_ - The descendant combinator — typically represented by a single space (" ") character — combines two selectors such that elements matched by the second selector are selected if they have an ancestor (parent, parent's parent, parent's parent's parent, etc.) element matching the first selector.

                header p {
                    color:red;
                    font-weight: bold;
                }

        2.  _Selector list_ - The CSS selector list (,) selects all the matching nodes. A selector list is a comma-separated list of selectors.

                header, p, div {
                    color:red;
                    font-weight: bold;
                }

        3.  _Child combinator_ - The child combinator (>) is placed between two CSS selectors. It matches only those elements matched by the second selector that are the direct children of elements matched by the first.

                header > p {
                    color:red;
                    font-weight:bold;
                }

    -   _CSS Pseudo-class_ - [HERE...](https://www.w3schools.com/css/css_pseudo_classes.asp)
    -   _CSS Pseudo-element_ - [HERE...](https://www.w3schools.com/css/css_pseudo_elements.asp)

3.  Adding CSS to HTML - There are three ways of inserting a style sheet:

    -   External style sheet:

        -   An external style sheet is ideal when the style is applied to many pages. With an external style sheet, you can change the look of an entire Web site by changing one file. Each page must link to the style sheet using the tag.
        -   The tag goes inside the head section:

                <head>
                    <link rel="stylesheet" type="text/css" href="style.css">
                </head>

    -   Internal style sheet:

        -   An internal style sheet should be used when a single document has a unique style. You define internal styles in the head section of an HTML page, by using the style tag.

                <head>
                    <style>
                        body{
                            ...
                        }
                    </style>
                </head>

    -   Inline style:

        -   An inline style loses many of the advantages of style sheets by mixing content with presentation.
        -   Do not use this method unless you have no other choice.
        -   To use inline styles, you use the style attribute in the relevant tag. The style attribute can contain any CSS property.

                <div style="color: red;">
                        …
                </div>

4.  CSS Selector Inhertance & Specificity:

    -   CSS relies heavily on specificity and style overwriting.
    -   It's in the name!.
    -   Cascading Style Sheets.

        <img src="https://cdn.rawgit.com/MakeSchool-Tutorials/sa-2018-landing-page/master/P06-CSS-Inheritance-And-Specificity/assets/class_specificity_value.png" width=450px >

    -   Cascade Order - in increasing order of priority.
        1. External <link>
        2. In the <head>
        3. Inline style attribute
        4. Using !importan

5.  CSS Properties:

    -

6.  Practice
    -   some zip files with solutions (homework)
    -   more exercises

## 2. Typography in CSS.

1.  **What is Typography?** - Typography is the art and technique of arranging type to
    make written language legible, readable, and appealing when displayed.Typography is the visual component of the written word.

    -   _Styling text_ - Choosing a comfortable measure
        -   The measure is the number of characters in single line of a
            column of text.
        -   Anything from 45 to 75 characters is widely regarded as a satisfactory length of line for a single-column page set in a serifed text face in a text size.
        -   The 66-character line (counting both letters and spaces) is widely regarded as ideal. For multiple column work, a better average is 40 to 50 characters.
    -   _Fonts & Font Famiy_
        -   Font Family:
            -   In typography, a font family (also known as typeface) is a set of one or more fonts each composed of glyphs that share common design features.
            -   Each font of a typeface has a specific weight, style, condensation, width, slant, italicization, ornamentation, and designer or foundry.
        -   Font:
            -   A computer font (or font) is implemented as a digital data file containing a set of graphically related glyphs, characters, or symbols such as dingbats.
            -   Although the term font first referred to a set of movable metal type pieces in one style and size, since the 1990s it is generally used to refer to a set of digital shapes in a single style, scalable to different sizes.
        -   Generic Font Families:
            -   serif
            -   sans-serif
            -   monospace
            -   cursive
            -   fantasy
        -   Web Fonts:
            -   At the time, fetching font files from the web was controversial because fonts meant to be used only for certain web pages could also be downloaded and installed in breach of the font license.

2.  **CSS Units**

    -   _EM & REM:_

        -   Ems are so-called because they are thought to approximate the size of an uppercase letter M, although 1em is significantly larger than this.

         <img src="https://www.pc-koubou.jp/magazine/wp-content/uploads/2019/10/css_rem_main2.png" width=350>

        -   The em is a sliding measure. One em is a distance equal to the type size.
        -   In 6-point type, an em is 6 points; in 12 point type an em is 12 points and in 60 point type an em is 60 points.

3.  **CSS Properties**
    -   _color & background_ - comes together!
    -   _text:_
        -   text-align: left,right,center ...
        -   text-decoration: - decorate the text
        -   text-indent: - move the text with space
        -   text-overflow: - if the text is more than the box
        -   text-shadow: 0 0 5px black - shadow of the text
    -   _font:_
        -   font-family: serif etc. - type of the font
        -   font-size: 2em - font size
        -   font-style: italic - style of the font
        -   font-weight: 700 - weight of the font
        -   line-height: 1.5 - space between lines

[BACK](#contents)

## 3. Box Model & Positioning

[BACK](#contents)

## Demo

<!-- 1. [my first HTML page](https://github.com/baiGeorgi1/baiGeorgi1) -->
