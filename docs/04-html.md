# HTML Recitation

## Using your Text Editor to Hard Code a Web Page

1. Right click on your desktop and create a folder.
2. Name the folder task02-01.
3. Open up your text editor. (It is helpful to use a text editor that has a project sidebar to follow along in class. VS Code and Brackets show project files in a sidebar.)
4. Open the folder:
   * Drag the folder onto your text-editor side bar,
   * or choose to open the folder using the menu or icons.
   * Any changes you make in the sidebar will affect the file on your desktop and vice-versa.
5. Right click in the sidebar and create a new file. Name it ```index.html```.
6. Right click in the sidebar and create another new file. Name it. ```notes.txt```.

## Use a Browser to see your page develop

You will need to open up a browser to view your progress as you go along.

From within your editor sidebar, you can open the folder on your desktop. (This can be helpful if you have your folder in a subfolder.) To do this, right click on your ```index.html``` file name and choose reveal in finder. You can double click the file and it will open in your default browser. If you do not wish to open the file with the default browser, drag the ```index.html``` file onto the desired browser window.

At this point in the class you should be able to follow along with the class demo.

1. We will start coding in the ```notes.txt``` file to see how the text behaves there.
2. Then we will code some in the ```index.html``` file to see if the text behaves any differently.

This will introduce the concept of an **IDE: an integrated development environment**. You will see that your text editor is more "helpful" with html suggestions if you are working with an html file.

## Saving

Remember that you must save the file in your editor before you can preview your code in a browser. Look for the little dot next to the file name in the top tab.

## Caching

Beware of “caching.” Web browsers will sometimes, but not always, save a copy of your webpage that is essentially invisible to you. The reason for this is to save resources everywhere; time, server hardware, client hardware. Electricity is needed to drive the web. caching makes sites faster and more affordable for everyone. But it can really be a big headache when you are creating websites.

**Solution:** Proof your site in incognito or private mode.

## Viewing code in a browser

Right-click on web page and choose view source to see your code. Be careful not to right-click on an image. If you do, you will see the image property data, and not the code.
Put all of your files in one "Root" folder

Images, PDFs pages all must be in the root folder. Copy all of you images into the root folder. Avoid linking to images on the web not in your folder. That is called “hotlinking” and makes your page dependent on that server. If you don't have permission to "hotlink" then you are effectively [stealing bandwidth](https://www.keycdn.com/support/what-is-hotlinking). It is okay to link to an image that directs you to that page.

## Uploading your files to Opal with SFTP

**The text editors that we are using do not allow for file uploading. You will need to use your sftp program.** Remember that you need to put your folder in the ```public_html``` folder for it to be visible via a web browser.

To log into opal with your SFTP program enter ```opal.ils.unc.edu``` for the server and your username is your ```onyen```. Your password is your onyen password. After you upload your folder to the public_html directory in opal, you will need to direct your browser to ```https://opal.ils.unc.edu/~youronyen``` to confirm it has uploaded correctly uploaded.h
