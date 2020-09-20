# Templates

## Wrap up 02.02 Task

If you are still having issues with this task, please try to get up a bit early and work with me before class or meet with me after class. I can spend a few minutes of class time on simple issues, but if you are dealing with a complex problem, we will need to meet after class or set up office hours.

If you need a review, look over the the Sep 07 CSS class notes (link in left sidebar). We all missed this class due to the Labor Day Holiday. If you need to look at the videos again, go to the class entry [in the calendar](https://sakai.unc.edu/x/LOzYFh) to access the videos. *You will default to the current week, so go to the previous week.*


!> your home page, or initial page should always be named **index.html**. the "i" should be lower case and html should be lowercase. Don't name it **index1.html** or **2index.html**. Don't ever have a page named **home.html**. Your **home** page **is** the **index.html** page. If you name it with a capital "I" the browser OPAL will not hide it in the directory. It will be listed like any other non index.html file.

## Navigation

Navigation design basics are the most crucial next step to learn after getting HTML and CSS basics down. Navigation design is complicated. Especially when building responsive sites. We don't have time to go into the fine details. But I do want to go over some absolute basics. You do not have to follow along with me, but I will create a project and demonstrate this in class. It's your choice follow along or just watch. If you complete this task and post it on opal it will give you credit for both task 02.01 and 02.02, so if you are behind, you can get caught up today.

```
<!DOCTYPE html>
<html>
 <head>

  <title>Navigation Example</title>
   <!-- <link rel="stylesheet" href="style.css"> -->
   <!-- <meta name="viewport" content="width=device-width, initial-scale=1.0"> -->
   <!-- <meta charset="utf-8"> -->
   <!-- <link href="https://fonts.googleapis.com/css2?family=Spectral:wght@300&display=swap" rel="stylesheet">  -->
 </head>
 <body>
<!-- Start of Navigation code -->

  <ul class="topnav">
   <li><a class="active" href="index.html">Home</a></li>
   <li><a href="about.html">About</a></li>
   <li><a href="classes.html">Classes</a></li>
   <li><a href="interests.html">Interests</a></li>
  </ul>

<!-- End of Navigation code -->  
  <article>
   <h1>{Home} Page</h1>
    <p>This is the {Home} page.</p>
    <p>If you duplicate the page to make a new page, you need to edit the active link class,
       the title, the h1 and the p content for all pages.</p>
  </article>

 </body>
</html>
```

This is the associated CSS code:

```
body {
  margin: 0;
  font-family:'Spectral', serif;
  font-size: large;
  background-color: tan;
}

article {
  margin:3% 5% 5% 10%;
  background-color: white;
  padding: 3%;
  border-radius: 5px;
}

ul.topnav {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

ul.topnav li {float: left;}

ul.topnav li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

ul.topnav li a:hover:not(.active) {background-color:tan;}

ul.topnav li a.active {
  color: black;
  background-color:tan;}

ul.topnav li.right {float: right;}

@media screen and (max-width: 600px) {
  ul.topnav li.right,
  ul.topnav li {float: none;}
}
```
## Choosing a Template

By now you should understand the basic HTML structure and how CSS is used to make the basic HTML more visually pleasing. In 2020 web designers should be using themes that will work on phones. This is called responsive design. Your template will contain CSS code that can take advantage of different screen sizes. I would encourage you to look for keywords that mention "mobile", "responsive" or "mobile friendly" in the template description. I will not downgrade you for using a non-mobile theme, but users will not like your site if they view it on a phone.

Take a look at the following code and note the comments:

```
<!DOCTYPE html>
<html lang ="en"> <!-- english language attribute added -->

  <head>

    <!-- utf-8 character set helps browser display text correctly -->
    <meta charset="utf-8">

    <!--  this view port setting makes for better display on mobile devices -->
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <!--  link assumes you have a stylesheet containing styles in a directory named styles -->
    <link rel="stylesheet" href="styles/style.css">


    <title>Student Name | Home Page</title>
  </head>

  <body>
    <p>Welcome to my webpage! This is my only page. This is not an website.</p>
  </body>
</html>

```

## Working with Templates

Here are a few examples of my own templates that some students have used from past classes (these have the mobile friendly settings in the ```<head>```).

* [One page template sample](https://opal.ils.unc.edu/~lblakej/website-helps/02-one-page-final-sample/) | [Download one page template](https://opal.ils.unc.edu/~lblakej/website-helps/03-one-page-source-files/one-page-green-starter-theme.zip)
* [Multiple page template sample](https://opal.ils.unc.edu/~lblakej/website-helps/05-multi-page-final-sample/) | [Download multiple page template](https://opal.ils.unc.edu/~lblakej/website-helps/06-multi-page-source-files/multi-page-template.zip)
* [UNC Theme Sample](https://opal.ils.unc.edu/~lblakej/website-helps/07-NEW-bootstrap-template/index.html) | [Download Bootstrap-based UNC theme template](https://opal.ils.unc.edu/~lblakej/website-helps/07-NEW-bootstrap-template/)
* [Background Photo Sample](https://opal.ils.unc.edu/~lblakej/website-helps/08-example/about.php) | [Download Bootstrap-based Photo Theme template](https://opal.ils.unc.edu/~lblakej/website-helps/08-template.zip)


A lot of students also used templates from the [sources on the class web site](https://ils.unc.edu/courses/2020_fall/inls161_001/06a.01.preps.html).

In class we will download some different themes and discuss all of elements that you will need to include in your website to earn full points. The class will be recorded.
