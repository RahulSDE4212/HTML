## **WHAT IS HTML**
- `HTML` stands for **HYPER TEXT MARKUP LANGUAGE**.
    - `Hyper-Text` : A special type of text document in which you can put hyperlink of another text document.
    - `Markup Language` : Text-encoding system which specifies the structure and formatting of a document.

- `HTML` - not a programming language. Anything to be called as a programming language must support the decision making (if, else etc.) which HTML doesn't support.
- `HTML` provides the skeleton of a webpage.
- Example of Markup language - **HTML, Markdown**.
- The basic building blocks of **HTML** is `Tags`.

```
    <!DOCTYPE html>    -> this represents that the web browser expect what type of html document.
    <html lang = "en"> -> this represents that the language of html is english.
    <head>             -> this tag is used to add extra information with out html document.
        <meta http-equiv = "X-UP compatible content = "IE-edge">
        <meta name = "viewport" content="width=device-width, initial-scale=1.0">
        <title>Rahul</title>  -> this tag will show Rahul on the top of web browser.
    </head>
    <body>
        whatever will be added here will be added to the web page
    </body>
    </html>
```


## **TAGS**
- a single mechanism using which you can tell what is this part of document actually meaning. 
- **Syntax:**
    ```
        <tag name> some information </tagname>
           |                            |
        opening tag                    closing tag
    ```
- Tag is the syntax that we actually use in order to write the html code, when the tag is dispalyed on the browser, it beomes html element.
- With a tag, there is an opening and closing tag associated with it.
- There is an exception. There are some tags which are self-closing tags means we don't need to put closing tag with them.
    - ex:
    ``` 
        <tagname>
             |
        Here opening and closing is managed by same tag
    ```

### **DIFFERENT TYPES OF TAGS**

### **HEADING TAGS**
- 
    ```
        <h1> this is heading 1 </h1>
        <h2> this is heading 1 </h2>
        <h3> this is heading 1 </h3>
        <h4> this is heading 1 </h4>
    ```
- Used to put heading in the docs which is in bold colour.

### **PARAGRAPHS TAGS**
- 
    ```
        <p> this is paragraph </p>
    ```
- Used for paragraphs.
- The text will be in normal colour.

### **LIST TAGS**
- There are two types of list tags.
    ```
              List in HTML 
                  |
        -------------------------
        |                        |
    unordered                  ordered
    . list item 1             1. list item1
    . list item 2             2. list item2
    . list item 3             3. list item3
    . list item 4             4. list item4
    SYNTAX:                  SYNTAX:
        <ul>                   <ol>
         <li>item1</li>           <li>item1</li>
         <li>item2</li>           <li>item2</li>
         <li>item3</li>           <li>item3</li>
        </ul>                  </ol>
    ```
- Used to put heading in the docs which is in bold colour.

### **IMAGE TAGS**
-  Syntax:
    ```
        <img src= " " alt= " "/>
    ```
- Image tag is a self-closing tag.
- There are many attributes associated with this tag to show characterstics of image.
- `src = " " `  : Here in the inverted comma, we write the path/ address of image where it is actually present.
- `alt = " " `  : Here we write the description of image, which screen reader will read for blind people.

``` 
Inline tag                               Block tag
   |                                          |
a tag which always put the              a tag which always put
info of next tag in the                 the info of next tag 
same line.                               int the new line. 
```
### **DIV TAGS**
- Syntax
    ```
        <div>
            one divtag
        </div>
        <div>
            hi there
            <img src=" " alt=" "/>
        </div>
    ```
- used to write the general statement mix with anything.
- It is an block tag.

### **SPAN TAGS**
- Syntax
    ```
        <span> There is span1 </span>
        <span> There is span2 </span>
    ```
- used to write the general statement mix with anything in the same line..
- It is an inline tag.

### **AUDIO AND VIDEO TAGS**

### **MARQUEE TAGS**
- webpage me line ko ek taraf se dusre taraf i.e. moving line create karne ke liye use hota hai.
- Syntax:
    ```
    <marquee behaviour = "scroll" direction = "right"> TEXT </marquee>
    ```

### **INPUT TAGS**
- Syntax:
    ```
     <input type = " " />
    ```
- Self-closing tags.
- There are different types of attributes associated with input tag.
    - `<input type = "text"/>`
    - `<input type = "button" value = "what should be printed on button"/>`
    - `<input type = "color"/>`
    - `<input type = "checkbox"/>`
    - `<input type = "date-time-local"/>`
    - `<input type = "number"/>`
    - `<input type = "radio"/>`

### **SELECT TAG**
- Syntax:
    ```
    <select>
        <option>India</option>
        <option>china</option>
        <option>uk</option>
    </select>
    ```
- This is an input tag that is used for:
    - Different options are available in drop-down and we have to select one. 

### **TEXTAREA TAG**
- Syntax:
    ```
    <textarea rows = "30" cols = "25"></textarea>
    ```
- this is an input tag which provides an area to write the text and that area 
  can be increased or decreased.

### **TABLES IN HTML**
- used to create a table.
- Syntax:
    ```
    <table border = "1" cellpadding = "10px" cellspacing = "10px">
    <thead>
       <tr> Heading of the table </tr>                                              Heading of the table
    </thead>                                                                   ----------------------------------
    <tbody>                                                                    |   one         |        two     |
        <tr>                                                                   ----------------------------------
            <td>one</td>                                                       |   three       |     four       |
            <td>two</td>                                                       ----------------------------------
        </tr>
        <tr>
            <td>three</td>
            <td>four</td>
        </tr>
    </tbody>
    </table>

### **FORMS TAG IN HTML**
- Syntax:
    ``` 
    <form>
        <input type ="text" placeholder = "name">
        <input type ="number" placeholder = "age">      
        <input type ="submit" value = "clickme!!">         
    </form>
- This tag is used to collect data/input from the user.
- Inside the form tag we will use only those tag which is used to take input from the users.
- `<input type="submit">` : This will submit the data entered by user in form tag in the backend where logic for collection of data is written

    - ### **Attributes associated with INPUT TAG.**
        - #### **placeholder Attributes**
            - Syntax:
                ```
                <input type = "text" placeholder="name">
                ```
            - It gives hint to the user that what this input part is actually accepting.
            - Temporary display value.

        - #### **VALUE Attributes**
            - It is the actual text that the HTML put with input.
            - Ex:
                ```
                <input type="submit" value="click">
                <input type="text" value="India" placeholder="country">
                ```
        
        - #### **disabled Attribute**
            - make the html element disabled.
            - Syntax:
                ```
                <input type="submit" value="Disabled button" disabled = "xyz">
                ```
        
        - #### **name attributes**
            - with the help of name attributes we can check that whatever the input is given by user is of which thing.
            - Syntax:
                ```
                <input type = "text" placeholder="name" name="first name">
                ```


