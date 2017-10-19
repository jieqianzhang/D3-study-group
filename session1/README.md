First of all, you need a text editor, please download Sublime from here: https://www.sublimetext.com/3 

# Basical HTML 

## Vocabulary words for HTML
Developer Tools / Web Inspector / Dev Tools

HTML tags

DOM

Attribute

### Developer Tools / Web Inspector / Dev Tools
By using web inspector in browsers, you can inspect the “DOM” or Document Object Model. It’s displaying the underlying **LIVE REALTIME** HTML code for the web page, which is different than the static HTML document you’ve written.

### HTML tags
Opening Tag ``<p>``

Closing Tag ``</p>``

Block elements: div, h1, p, ul, li

Inline elements: span, a, img, strong, em

### Attributes
Attributes are pieces of information that can go into tags.
For example: 
```<a href="https://www.wsj.com"></a>```
``href=""`` go inside the <a> tag to specify where a user will go when they click a link.
  
Attributes to use for CSS:
There are three attributes that can go in HTML tags: 
id attibute — This is a unique term that gives this tag an identifier we can reference in our CSS.
class attribute — This is a grouping term that allows us to reference multiple tags in our CSS.
style attribute — This is a special way to include inline CSS, basically putting CSS code directly into an HTML tag.

#### Data Attribute

The data attribute will be important later when we do JavaScript. This attribute allows us to include some arbitrary data to HTML tags, which can be used by plugins or many other JavaScript utilities.

Data attributes always start with the word data and then end with a hyphen. The words that come after that depend on the plugin being used. There might be a plugin that wants the word “slideshow” as a data attribute. In your html tag, you might include: data-slideshow="true" The data keyword here is slideshow, and the value you assign it is true.


# What is CSS
CSS stands for **Cascading Style Sheets**, and there is a reason why. The language is built on the idea that there will be conflicts among the different rules. Like with the general selector, which affects all HTML tags in your document, you can override earlier rules.

The cascade refers to a set of parameters whereby one rule overrides another. Here are the general parameters:

* Last Rule: If two identical rules are setup with the same weight, the one that comes last wins out.
* Specificity: If one selector is more specific, it wins out (even if it comes before another).
* !Important: Use this as a last resort. You can override individual styles with an !important declaration at the end of the property, but before the semicolon close.
```
<h1 id="headline">Headline Goes Here</h1>

```

```
h1{
    font-size: 48px; 
    color: red; 
}
```

```
#headline{
    color: black;
}
```

```
h1{
    color: yellow; 
}
```

Question: What color is our headline? 

## selector 
* ``h1``, ``h2``, ``h3``	Type Selector - Matches to elements of specified name, regardless of where they are.
* ``.note``	Class Selector - Matches any number of elements with a class attribute of the same name.
* ``#headline``	ID Selector - Matches only one element that has an id attribute of the same name.
* ``li > a``	Child Selector - Matches elements that are one-level direct descendant of the other.
* ``p a``	Descendant Selector - Matches elements at any level below the first listed selector.


# Learning the Terminal 
The Terminal program on the Mac is a window into the command-line interface (CLI). This is the ability to interface with your computer using text commands, much the way it was done on Unix/Linux computers.
### Listing files in the Terminal ``~$ ls``
### Navigation around the file system  ``~ $ cd Desktop``
The dot ``.`` means the current directory.
The double dot ``..``means the parent directory.
The tilde ``~`` always points to your home folder.
### Start a localhost
First to make sure which version of python you have on your computer
``python -V``
Then start a localhost by typing in: 
``python -m SimpleHTTPServer 8000``

# Javascript
## variables
The **var** keyword and assignment operator 
```
var x = 7;
```

## array
An array is a method of storing multiple values in a single variable.
``var myarray = ["steph", "renee", "max", "josh"];``

## console
``console.log( myarray[2] );``

## object 
An object literal is written with curly braces. Each item in the object contains an keyword called a property and it is separated by a colon with the value of that property.
``var person = {name: "steph", age: 28, location: "New York"};``
`` console.log(person.name)``
Or you can access the data by using: 
`` console.log(person["name"])``

## JSON
There is a standard on the web for transferring information between websites called JavaScript Object Notation, or JSON. It is simply a combination of JavaScript object notation and arrays. JSON is used by many other programming languages than JavaScript, and has cemented itself as a standard format for data. This is why understanding objects, arrays and datatypes is so crucial for understanding how JavaScript works.

```
{
    "firstName": "Stephanie",
    "lastName": "Stamm",
    "age": 28,
    "address": {
        "streetAddress": "xx xx Street",
        "city": "New York",
        "state": "NY",
        "postalCode": "10021"
    },
    "phoneNumber": [
        {
            "type": "home",
            "number": "123456789"
        },
        {
            "type": "fax",
            "number": "123456789"
        }
    ]
}
```



# Set up D3 
## include a script tag and link to D3 script 
```js
<script src="https://d3js.org/d3.v4.min.js"></script>
<script>    
    Your code here
</script>
```
## Enter data 


## Draw a bar chart 
