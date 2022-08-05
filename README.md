# Introduction
* Inline n Block Elements
    * Inline elements cant have some style properties that blocks have such as height and weight. However they can be identified like block such as :
    ```
    <b style="
        display: inline-block;
        height: 50px;
        ">example</b>
    ```
* Some display types: initial, inherit, none, inline, inline-block, block, list-item, table, table-row, table-cell, flex, inline-flex

* When inspecting on browser Styles is the part what I identified for elements and Computed is what is identified automatically by browser.

* Basic Selectors
    * universal selector: (*)
    * type selector: (input,h1)
    * class selector: (.classname)
    * id name selector: (#id)
    * attribute selector: (  [class] {color: red};  ,   [id] {color: blue};   )

# Blog Design

* CSS can be added to HTML documents in 3 ways:
    * **Inline** - by using the ```style``` attribute inside HTML elements
    * **Internal** - by using a ```<style>``` element in the ```<head>``` section
    * **External** - by using a ```<link>``` element to link to an external CSS file


    ```
    <!DOCTYPE html>
    <html>
    <head>

    <link rel="stylesheet" href="styles.css">
    
    </head>
    <body>

    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>

    </body>
    </html>
    ```
* Size unit "em" is better for scaling 
    ``` 
    1 em = 16px 
    ```
* CSS helper classes, also known as utility classes, are used as,
    ``` 
    .gray {
    color: gray;
    }

    .ff-sans {
    font-family: sans-serif;
    }

    <h3 class="gray ff-sans">
        something grey n sans serif
    </h3>
    ```
# Form Elements

* When label is clicked it focuses on associated element.
<br>

* Label for references the id of anything associated. If label tag contains the associated element, then no need id and for.<br> 
Below examples mean same thing.

    ```
    <form action="">
        <label for="name">Name</label>
        <input id="name" type="text" />
    </form>
    ```

    ```
    <form action="">
        <label> Name <input type="text" /> </label>  
    </form>
    ```
* Input type declares what is expected. In mobiles, suitable keyboard opens due type, such as numbers or words.

* If radio type inputs have same name, only one can be chosen at a time. Using "checked" makes one of them default.

* Input value and name is important while posting the form. Name works as key.

* Some selector identifications in CSS for components and actions;
    ```
    input[type="email"]::placeholder,
    textarea::placeholder {
    color: rgb(175, 175, 175);
    }

    input[type="email"]:focus,
    textarea:focus {
    border-color: rgb(68, 176, 255);
    }

    :focus {
    outline: 0;
    }
    ```

* Icon that is used on background can be pixel fixed as background-size;
    ```
    select {
    -webkit-appearance: none;
    background-image: url("angle-down.png");
    background-repeat: no-repeat;
    background-size: 17px;
    background-position: right 10px center;
    }
    ```

* "+" sign can be used to mean "if some elements comes one after another" in CSS;
    ```
    .radio-container label + label {
    margin-left: 10px;
    }
    ```

* .form-row > label -->affects one-down position children so it doesn't include the lower label tags.

# Box Sizing

* Box sizing is used to keep child container inside of parent container.<br>
 It handles problems about border but wont affect margin.

* Therefore, at start of a project applying box sizing as below to make some adjustment is useful for smooth working.
    ```
    * {
        box-sizing: border-box;
    }
    ```

* In this example (*) refers to universal selector. 

* Parent containers padding works as margin of the child container.

# Reset.css and Normalize.css

* This adjustments must be in the first line of CSS

* Reset.css disables all the auto-stylings in browsers and makes view exact in all browsers

* Normalize.css only provides similarity in browsers and keeps auto styling for practicality.

* Normalize.css can be imported in CSS by url
    ```
    @import "https://necolas.github.io/normalize.css/8.0.1/normalize.css"
    ```
* 


# ?
* What about https://httpbin.org/forms/post
* something is not working in .radio-container label + label in form elements