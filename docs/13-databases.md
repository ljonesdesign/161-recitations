# Databases

## Relative, Absolute, and Mixed References

Before we discuss the VLOOKUP function, we need to be aware of absolute and relative cell references. If you want to learn more:

* Here is a [link that details the difference between relative and absolute references](https://support.microsoft.com/en-us/office/switch-between-relative-and-absolute-references-981f5871-7864-42cc-b3f0-41ffa10cc6fc), and
* Here is a [video that goes over Relative, Absolute, and Mixed References.](https://www.youtube.com/watch?v=FRu48zy-Djk)

*It is not necessary to have watched the video to follow along in class.*

!> Short version: we must use absolute references in our lookup data range. Excel uses relative references by default. To make a column or row reference absolute, manually place a dollar sign ($) in front of the reference. You may also cycle through the choices by clicking in the formula bar ![formula bar](images/formula-bar.png) and typing ```mac: command + T``` or ```pc: fn + F4```.  
<br>See Table 1 for examples.

**Table 1**

Type | Cell | Action
---:|---|---
Relative Reference: | A2  | None; default in Excel
Absolute Reference: | <b>$</b>A<b>$</b>2 |  enter dollar sign in front of column <b>and</b> row reference
Mixed Reference: | <b>$</b>A2 or A<b>$</b>2 | enter dollar sign in front of column <b>or</b> row reference



## VLOOKUP Demo

Here is an excel file you can download if you want to follow along in class: [VLOOKUP Examples](https://github.com/ljonesdesign/161-recitations/raw/master/docs/files/jones-vlookup-examples-v2.xlsx). I put in some Star Wars and Harry Potter data to make it a little more fun. We will practice this a lot.

With all that practice, you can now go download the file for your [VLOOKUP task](https://github.com/ljonesdesign/161-recitations/raw/master/docs/files/spreadsheets.vlookup-example.xlsx) and get in done in a minute.

## SQL

It's pronounced ess-que-el, and it stands for Structured Query Language.

This is the main thing you need to take away from this recitation &mdash; you select a **field** (AKA column), from a **table**, **where** some sort of condition, or conditions, can be matched. And if you want, you can **order** (or sort) your data from ASC ascending, or DESC descending.


```
SELECT column1, column2, ...
FROM table_name
WHERE condition;
ORDER BY DESC
```


For example, if you used SQL to find all book titles in a book database that contained the word `freedom` you would have to know what table in the database contained all the book titles.

1. If you looked in a full output from the author table you would not find any titles:

    * [tblAuthor](https://trianglewebs.com/book-database/tblAuthor.php)
    * In this output, you only have the results, so you don't even know what the column name is for the author.

2. Nor would you find the title in a full output of the publisher table:

    * [tblPublisher](https://trianglewebs.com/book-database/tblPublisher.php)

3. If you looked in the book table you would finally find the listed titles:

    * [tblBook](https://trianglewebs.com/book-database/tblBook.php)
    * However, you should not trust that the html headings are the actual database field (column) names. They might just be labels. One clue that they are not
    trustworthy is that some of the headers contain spaces: ```LOC Number``` and ```Pub FK```. Notice that the SELECT statement example
    is looking for ```column1, column2```. When you named your table in your VLOOKUP exercise, Excel would not allow you to put in a space or a hyphen. **It would allow an underscore.** Underscores are very common in Database column names.

    TLDR; the actual field name for the book title is ```tblBook_Title```.

4. Here is a [link to a reference page](https://trianglewebs.com/book-database/index.php) to our book database. Here you can find all of the tables and all of the column heads ("field names" are more appropriate when discussing databases.)

5. The reference page has a lot of information that will help you get started with writing your own SQL statements. I will demo several in class. There is a cut and paste example that you can use to find titles that contain the word `freedom`.

## SQL Tasks

*This will require you to have the [help page](https://trianglewebs.com/book-database/index.php) open in a window, the [SQL entry page](https://trianglewebs.com/book-database/sql-entry.php) open in a window and this page open in a window.*

### Create three SQL queries

#### Query 01:
select all the titles from ```tblBook``` where the ```language``` is ```German``` and include both the titles and the language in the result.

>If your query is successful, paste a copy of the query in ```cell N1``` on your ```05-Summary worksheet```

#### Query 02:
select all the names from ```tblPublisher``` where the ```city``` is like ```Berlin``` and include both the name and the country in the result

>if your query is successful, paste a copy of the query in ```cell N2``` on your ```05-Summary worksheet```

#### Query 03:
select all the titles from ```tblBook``` where the ```topic``` includes the word ```Virginia``` and include both the titles and the topic in the result, sorted by the title

>if your query is successful, paste a copy of the query in ```cell N3``` on your ```05-Summary``` worksheet
