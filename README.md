# HTML-CSS

HTML &amp; CSS course - January 2024

## Contents

1. [Introduction to HTML & CSS.](#1-introduction-to-html--css)
2. [Typography in CSS.](#2-typography-in-css)
3. [Box Model & Positioning](#3-box-model--positioning)
    1. [What is Box Model?](#1-what-is-box-model)
    2. [The CSS Box Model](#2-the-css-box-model)
    3. [Position](#3-position)
    4. [Resourses](#4-resourcesbox-model--position)
4. [CSS Layout - Flexbox]()

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
        1. External `<link>`
        2. In the `<head>`
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

         <img src="https://www.pc-koubou.jp/magazine/wp-content/uploads/2019/10/css_rem_main2.png" width=350px>

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

#### 1. **What is Box Model?**

-   When laying out a document, the browser's rendering engine represents each element as a rectangular box according to the standard CSS basic box model.CSS determines the size, position, and properties (color,background, border size, etc.) of these boxes.

    [...more info](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)

      <img src="https://www.webcodzing.com/uploads/2021/06/box-model.jpg" width= 50% >

    -   _Display:_ - The display CSS property defines the display type of an element, which consists of the two basic qualities of how an element generates boxes.

        -   the outer display type defining how the box participates in flow layout;

        -   he inner display type defining how the children of the box are laid out;
            <img src="https://miro.medium.com/v2/resize:fit:828/1*8-ZiQE4l2YY_ddk5yW8Ujg.png" height=250px>

        1.  display: block;
            -   TML elements historically were categorized as either "block-level" elements or "inline" elements.
            -   By default, a block-level element occupies the entire space of its parent element (container), thereby creating a "block".
            -   Browsers typically display the block-level element with a newline both before and after the element.
            -   You can visualize them as a stack of boxes.
        2.  display: inline;
            -   Inline elements are those which only occupy the space bounded by the tags defining the element, instead of breaking the flow of the content.
        3.  display: inline-block;
            -   Gives us the ability to use vertical padding and margin on inline elements as well as adding width and height.

    -   _Width:_ - The width CSS property sets an element's width. By default,it sets the width of the content area, but if box-sizing is set to border-box, it sets the width of the border area.

        [more info...](https://interactive-examples.mdn.mozilla.net/pages/css/width.html)

        1. Default width of block elements:
            - If you don't declare a width, and the box has static or relative positioning, the width will remain 100% in width and the padding and border will push inwards instead of outward.
            - If you explicitly set the width of the box to be 100%, the padding will push the box outward as normal.
        2. min-width: ...px || em;
            - The min-width CSS property sets the minimum width of an element.
            - It prevents the used value of the width property from becoming smaller than the value specified for min-width.
        3. max-width: ...px || em;
            - The max-width CSS property sets the maximum width of an element.
            - It prevents the used value of the width property from becoming larger than the value specified by max-width.

    -   _Height:_ - The height CSS property specifies the height of an element.By default, the property defines the height of the content area.If box-sizing is set to border-box, however, it instead determines
        the height of the border area.

        [more info...](https://interactive-examples.mdn.mozilla.net/pages/css/height.html)

        1. min-height: ...px || em;
            - The min-height CSS property sets the minimum height of an element.
            - It prevents the used value of the height property from becoming smaller than the value specified for min-height.
        2. max-height: ...px || em;
            - The max-height CSS property sets the maximum height of an element.
            - It prevents the used value of the height property from becoming larger than the value specified for max-height.

    -   _Margin:_

        -   The margin CSS property sets the margin area on all four sides of an element.
        -   It is a shorthand for margin-top, margin-right,margin-bottom,and margin-left.

        [more info...](https://interactive-examples.mdn.mozilla.net/pages/css/margin.html)

    -   _Border:_

        -   The border CSS property sets an element's border.
        -   It's a shorthand for border-width, border-style, and border-color.

        [more info...](https://interactiveexamples.mdn.mozilla.net/pages/css/border.html)

    -   _Padding:_

        -   The padding CSS property sets the padding area on all four sides of an element.
        -   It is a shorthand for padding-top, padding-right, padding-bottom,and padding-left.

        [more info...](https://interactiveexamples.mdn.mozilla.net/pages/css/padding.html)

#### 2. **The CSS Box Model**

-   Block and Inline boxes:

    -   In CSS we have several types of boxes that generally fit into the categories of block boxes and inline boxes.
    -   The type refers to how the box behaves in terms of page flow and in relation to other boxes on the page.
    -   Boxes have an inner display type and an outer display type.
    -   In general, you can set various values for the display type using the display property, which can have various values.

    1. Outer display type - Inline:

        - If a box has an outer display type of inline, then:
            - The box will not break onto a new line;
            - The width and height properties will not apply;
            - Top and bottom padding, margins, and borders will apply but will not cause other inline boxes to move away from the box;
            - Left and right padding, margins, and borders will apply and will cause other inline boxes to move away from the box;
            - Some HTML elements, such as `<a>`, `<span>`, `<em>` and `<strong>` use inline as their outer display type by default.
        - The CSS box model defines how the different parts of a box — margin,border, padding, and content — work together to create a box that you can see on a page;

            - Inline boxes use just some of the behavior defined in the box model.

        - To add complexity, there is a standard and an alternate box model;
            - By default, browsers use the standard box model.

    2. Parts of a box:

    -   Making up a block box in CSS we have the:

        -   **Content box**: The area where your content is displayed; size it using properties like inline-size and block-size or width and height;
        -   **Padding box**: The padding sits around the content as white space; size it using padding and related properties;
        -   **Border box**: wraps the content and any padding; size it using border and related properties;
        -   **Margin box**: the outermost layer, wrapping the content,padding, and border as whitespace between this box and other elements; size it using margin and related properties;

            <img src="https://uploads.sitepoint.com/wp-content/uploads/2017/04/1492576965BoxModel1.png"  width=350px>

    -   In the standard box model, if you give a box an inline-size and a block-size (or width and a height) attributes, this defines the inlinesize and block-size (width and height in horizontal languages) of the content box;
        -   Any padding and border is then added to those dimensions to get the total size taken up by the box.
        -   If we assume that a box has the following CSS:
            -   The actual space taken up by the box will be 410px wide (350 + 25 + 25 + 5 + 5) and 210px high (150 + 25 + 25 + 5 + 5).
    -   In the alternative box model, any width is the width of the visible box on the page;

        -   The content area width is that width minus the width for the padding and border (see image below)
        -   No need to add up the border and padding to get the real size of the box.
        -   To turn on the alternative model for an element use:</br>
            `.box{box-sizing:border-box;}`
        -   If we assume the box has the same CSS as above:
            -   Now, the actual space taken up by the box will be 350px in the inline direction and 150px in the block direction.

        <img src="https://i.stack.imgur.com/4IT0d.png">

#### 3. **Position**

> The position property specifies the type of positioning method used for an element (static, relative, fixed, absolute or sticky)

> Elements are then positioned using the top, bottom, left, and right properties

> However, these properties will not work unless the position property is set first. They also work differently depending on the position value.

[more info...](https://developer.mozilla.org/en-US/docs/Web/CSS/position)

1. **position:static**;
    - The default state of every element — it just means"put the element into its normal position in the document layout flow — nothing special to see here."
2. **position: relative;**
    - Very similar to static positioning, except that once the positioned element has taken its place in the normal layout flow, you can then modify its final position, including making it overlap other elements on the page.
3. **position: absolute;**
    - This way we have to position the element based on a two dimentional coordinate system.
    - We can use left, top, bottom, right to place the element exactly where we want.
4. **position: fixed;**
    - The element is removed from the normal document flow, and no space is created for the element in the page layout.
    - The element is positioned relative to its initial containing block, which is the viewport in the case of visual media.
    - Its final position is determined by the values of top, right, bottom, and left.
    - This value always creates a new stacking context.
    - In printed documents, the element is placed in the same position on every page.
5. **position: sticky**
    - The element is positioned according to the normal flow of the document,and then offset relative to its nearest scrolling ancestor and containing block (nearest block-level ancestor), including table-related elements,based on the values of top, right, bottom, and left.
    - The offset does not affect the position of any other elements.
    - This value always creates a new stacking context.
    - Note that a sticky element "sticks" to its nearest ancestor that has a "scrolling mechanism" (created when overflow is hidden, scroll, auto, or overlay), even if that ancestor isn't the nearest actually scrolling ancestor.
6. **z-index**
    - The z-index CSS property sets the z-order of a positioned element and its descendants or flex items.
    - Overlapping elements with a larger z-index cover those with a smaller one.
    - [more info...](https://interactive-examples.mdn.mozilla.net/pages/css/z-index.html)

#### **4. Resources:Box model & Position**

1. Box Model:
    - https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model
    - https://developer.mozilla.org/en-US/docs/Web/CSS/display
    - https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing
    - https://css-tricks.com/the-css-box-model
    - https://css-tricks.com/box-sizing
    - https://www.paulirish.com/2012/box-sizing-border-box-ftw/
2. Position:
    - https://developer.mozilla.org/en-US/docs/Web/CSS/position
    - https://developer.mozilla.org/en-US/docs/Web/CSS/z-index
    - https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_positioned_layout/Understanding_z-index
    - https://interactive-examples.mdn.mozilla.net/pages/css/position.html
    - https://css-tricks.com/video-screencasts/198-about-the-position-property/
    - https://css-tricks.com/almanac/properties/p/position/
    - https://css-tricks.com/position-sticky-2/

[BACK](#contents)

## Demo

<!-- 1. [my first HTML page](https://github.com/baiGeorgi1/baiGeorgi1) -->
