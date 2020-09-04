# CSS

## HTML Review

This is the basic page that we hard coded last week. We did it line by line in notepad without any auto completion:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
   <title>Task 02.01 Assignment</title>
  </head>
  <body>
   <h1>Hard coded page.</h1>
   <p>This is a paragraph.</p>
  </body>
</html>
```
There is no CSS styling in the code above. (You can change the Title to 02.02 Assignment)

## Inline CSS

The best way to learn css concepts is to continue to hard code; however, cutting and pasting simple code is acceptable. Or you can use your autocomplete function in your text editor. Open up your last project and add some more code:

So let's put in some [inline css](https://codepen.io/lblakej/pen/RwajaEZ) with a style attribute.

Find the h1 tag and add this attribute: ```style="color:red;"```

Then, add some space like this:
```html              
<h1                   >Hard coded page.</h1>
```
Look at the box above. Notice how the first element closing bracket moved to the right. Every part of the attribute data has to go inside the first pair of brackets. Now look below. Look back and forth between these two boxes and confirm that ```style="color:red;"``` are in there in that particular order. This syntax will be repeated over and over with all of the other attributes that you will learn. Eventually, it will get easier to recognize the pattern.

```html            
<h1 style="color:red;">Hard coded page.</h1>
```
Notice that if the code is displayed on this page in a large gray box, the following will be true:

* green = <span style=color:#78a520;>attributes</span>
* blue = <span style=color:#2389b5;>attribute values</span>
* red (magenta) = <span style=color:#990055;>html</span>
* red can also be repeated in an attribute value if there is an <span style=color:#990055;>attribute value_1</span>:<span style=color:#2389b5;>attribute_value2</span> pair. (Look back to the inline style to see an example of this.) In this [codepen example](https://codepen.io/lblakej/pen/RwajaEZ), the pair is all one color.

Different text editors use different highlighting, but are consistent regarding elements, attributes, and values.

>Save your file with the changes, leaving the inline style in place. We need to keep that in the document to demo and discuss the concept of **cascading.** Preview your saved file in a browser to confirm that the heading is red.

This is what your code should look like after saving:
```html
<!DOCTYPE html>
<html lang="en">
  <head>
   <title>Task 02.02 Assignment</title>
  </head>
  <body>
   <h1 style="color:red;">Hard coded page.</h1>
   <p>This is a paragraph.</p>
  </body>
</html>
```


## Adding Styles in the head of the HTML Document

Inline styles are not optimal. It is **much** better to add them to the head of the document. But not the **best** way. We will get to the best way after this example.


Add this code block in the head:

```html
<style>
  p  {
    color:blue;
      }
</style>
```

Like this:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
   <title>Task 02.01 Assignment</title>
   <!-- below title -->
   <style>
    p  {
      color:blue;
        }
  </style>
  <!-- above the closing head tag -->
  </head>
  <body>
   <h1 style="color:red;">Hard coded page.</h1>
   <p>This is a paragraph.</p>
  </body>
</html>
```
>Leave the code as is and save and preview your file. Confirm that you have a blue paragraph and a red heading 1. If you add another paragraph element in the body, will it also be blue?

There are some situations where it is okay to put one or two styles in the head of the same document. But it is never optimal to put a lot of CSS code in the top of your document.

## CSS Placed in a Separate Document
The best way to add multiple styles to your webpage or website is to put the styles in a separate document and then link them to your web page or web pages.


Within your root folder, create a file named  ```style.css```.

*You can also name it as you wish. Examples might be ```main.css``` or ```primary.css``` or ```unc_theme.css``` but make sure you don't leave spaces or use bad naming conventions. Do try to make it understandable and relevant.*

In the new empty file enter a body tag and give it a background color of tan or choose another. [Here is a list of CSS Named background colors](https://www.w3schools.com/colors/colors_names.asp). There are only 140 named colors. All named colors can also be described in [HEX values](https://www.w3schools.com/colors/colors_hexadecimal.asp)

```css
body {
  background-color: tan;
}
```
!> Notice that you **do not** need to include the ```<style>``` tags if you are putting your styles in a separate css file.

It's time to address a common confusion before we go on... Linking a css file to an HTML file is very different than creating a text link out to [a funny cat gif](https://gfycat.com/hoarsetightcapybara). That is an **anchor link** and it looks like this:

```html
<a href="https:/gfycat.com/hoarsetightcapybara">a funny cat gif</a>
```

HENCE, why it starts with an **a**; a is for anchor. These anchor links have to go in the **body** of your html file. By the way, as you may have already found out, the link is not really a funny cat gif.

## Linking The webpage to the CSS File (Same level in folder)
Here is what the [HTML Link tag](https://www.w3schools.com/tags/tag_link.asp) looks like:
```html
   <link rel="stylesheet" href="style.css">
```
The link to a CSS file must go in the **head** of your web page. If you have multiple web pages that use the same css file, they also must include the exact same link in the head of the html page.

```
<!DOCTYPE html>
<html lang="en">
  <head>
   <title>Task 02.02 Assignment</title>    
   <link rel="stylesheet" href="style.css">
</head>
```

The file name must exactly match the file name you created, and, this is very important, it must be at the same level of your index.html or other html files, in the directory, for it to work as shown above.

```
- index.html
- style.css
```

## Linking to a Stylesheet (Stylesheet(s) in Directory in the root folder)

Look at the file set up below. There are two stylesheets in the stylesDirectory. You must reference them so that they can be found in the directory:

```
index.html
stylesDirectory
   style.css
   unc_theme.css
```
Here is how you link to just the style.css file:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
   <title>Task 02.02 Assignment</title>    
 <link rel="stylesheet" href="stylesDirectory/style.css">
</head>
```

Here is how you link to both style.css and unc_theme.css file:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
   <title>Task 02.02 Assignment</title>    
 <link rel="stylesheet" href="stylesDirectory/style.css">
 <link rel="stylesheet" href="stylesDirectory/unc_theme.css">
</head>
```
## Experiment with some css

You now know all you need to know to start experimenting with CSS. Have some fun! But make sure your CSS validates before you submit your 02.02 Assignment in Sakai.
