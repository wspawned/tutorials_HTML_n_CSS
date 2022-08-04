# Lecture Notes
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

* Normalize.css

* Basic Selectors
    * universal selector: (*)
    * type selector: (input,h1)
    * class selector: (.classname)
    * id name selector: (#id)
    * attribute selector: (  [class] {color: red};  ,   [id] {color: blue};   )

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

    Label for references the id of anything associated. If label tag contains the associated element, then no need id and for.<br> 
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

* Input value and name is important while posting the form.

# What about https://httpbin.org/forms/post ??
