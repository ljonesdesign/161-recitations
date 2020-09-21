# Website Checklist

Here is a checklist that you can use to make sure you have all the parts of your website done before posting to OPAL and submitting.

!><kbd>Control+F</kbd> (PC) and <kbd>Command+F</kbd> (Mac) will help you find what you are looking for on this page if you get stuck building your site. <br>[Six Keyboard Shortcuts Every Computer User Should Know](https://lifehacker.com/six-keyboard-shortcuts-every-computer-user-should-know-5836288)

>This was posted Sunday, September 20, at 1:00 p.m. so students can benefit from it if they are working on their sites before class on September, 21. It could use some final proofing, but I don't have any more time to work on it this afternoon. This page will be a dynamic source of help over the next few weeks. If you have any suggestions or ways to make this list better, then let me know.

<ol>
<li>
Use Word to export a real or example <strong>resume</strong> in pdf format; save it to your web project folder. <a href="https://www.youtube.com/watch?v=3Y-GeTi472A">Not sure about this? See this video.</a>
</li>

<li>
Find a <strong>template</strong>, verify it works for you and start building your site. See <a href="/#/06-templates">last week's, class notes</a> for more information.
</li>

<li>
Confirm you have a <strong>home page file named</strong> <code>index.html</code>. You <em>should not</em> have a file named <code>home.html</code>. If you are using a one page type of theme, you will create sections. If you are using a multi-page theme, you will create pages.
</li>

<li>
Confirm you have an <strong>About Section or Page</strong>. If not, create one.
</li>

<li>Create an <strong>Interests Section or Page</strong>.</li>

<li>
Create a <strong>Classes Section or Page</strong>.
</li>

<li>
Home Page Content: email with an <a href="https://www.albionresearch.com/misc/obfuscator.php"><b>obfuscated email address generator</b>.</a> | <a href="images/obfuscated-email.png"><b>How to do it.</b>.</a>
(This is not needed if you have a working Google Form.)
</li>

<li>
Home Page Content: <b>Image or graphic that loads fast and gets attention</b>.</li>

<li>
About Page Content: Have some custom about info related to you. Add a <b>relative link to your resume file</b> in the code of your <code>about.html</code> page. If you saved it or put it in the right folder, you will be able to easily link to it. </li>

<li>
If you did not save or already put a pdf formatted resume in your website project folder on your laptop, drag a copy named
<code>yourlastname-yourfirstname-resume.pdf</code> into your project folder. You will need to link to this using a <b>RELATIVE</b> link. <a href="images/resume.png">See this static screen shot for help.</a> or <a href="images/resume.gif">check out this animated gif. </a> </li>

<li>
A <b>RELATIVE</b> URL points to a file within a web site:

```
<a href="firstname-lastname-resume.css">My Resume</a>
```
A <b>RELATIVE</b> URL can also point to a file within a directory in a web site:

```
<a href="files/firstname-lastname-resume.pdf">My Resume</a>
```

Don't use an absolute URL (contains an http:// link) to point to your resume on another server or even on the opal server:

```
<!-- don't do this: -->
<a href="http://www.example.com/firstname-lastname-resume.pdf">My Resume</a>
```
</li>

<li>
Classes Page Content: <b>Links to each class you are taking this semester</b>.
</li>

<li>
Interests Page Content: At least an <b>HTML ordered list</b>.

```
<ol>
 <li>book1</li>
 <li>book2</li>
 <li>book3</li>
 <li>book4</li>
 <li>book5</li>
 <li>book6</li>
 <li>book7</li>
 <li>book8</li>
 <li>book9</li>
 <li>book10</li>
</ol>
```
</li>

<li>
Third level pages or section: Three placeholder objects for links to tasks 3-5. <a href="images/project-links-one-page.png">Single page Example</a> and <a href="images/project-links-multi-page.png">Multipage example</a>.
</li>

<li>
Every page should have a page last updated object.

```
<p>
  <script>
    document.write("Page last updated on " + document.lastModified);
 </script>
</p>
```
</li>

<li>
Make sure your <b>all your navigation links work</b>.
</li>

<li>
One <b>client side script</b>. (Javascript example.) See the <a href="02-scripting.php">page for a new example</a> I have put up there.

!>This is a specific required rubric item distinct from other rubric items that may or may not use javascript.

</li>

<li>
One <b>server side script</b>. (Google Form or Google Fonts or Google analytics.)
</li>


<li>
Make sure that <b>all of your images</b> have <code>alt=&quot;Description&quot;</code> attributes.
</li>

<li>
Verify that you <b>do not have any spaces in file or folder names</b>. <em>I count this as failed validation score.</em>
</li>

<li>
Verify that your image names and your source code CASE/CASE case/case match: (<code>image.jpg</code> must point to <code>image.jpg</code>) (<code>image.jpg</code> cannot point to <code>image.JPG</code> on OPAL)
</li>

<li>
<b>Upload to Opal</b> with your SFTP progam.
</li>

<li>
Check <a href="https://validator.w3.org/"><b>HTML validation</b>:</a> Copy a link from your home page and paste in the  validation form</a>: (i.e. https://opal.ils.unc.edu/~onyen/my-website/index.html)
</li>

<li>
Check <a href="https://jigsaw.w3.org/css-validator/"><b>CSS validation</b>:</a> Use same URL (i.e. https://opal.ils.unc.edu/~onyen/my-website/index.html)
</li>

<li>
Do your best to <b>fix validation errors</b> that are obviously your code edits. If the issue is with your template, that will not count against you.
For example, if you are using a bootstrap template, there will be some CSS validation issues with the <code>bootstrap.min.css</code> file; but, you should not be touching that file, so it is not your fault. (Unless you did indeed edit it by accident.) There may be some issues with cut and page Google Font and Google Form code, as well. That will not affect your validation grade.
</li>

<li>
<b>Submit your assignment in Sakai</b>. Paste your url in the assignment text box. If you can&#39;t figure out your validation errors, mention that in the submission post.
</li>

</ol>
