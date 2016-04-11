# About the Slideshow Viewer #

I guess you're probably wondering why you'd want to use this program instead of something more generic like irfanview. That's totally cool! Because, IMO, this is way better.

I got frustrated with irfanview for two main reasons: it was too random (I'd get an instruction card either way too frequently or way too infrequently), and the whole slideshow creation process was a pain.

So, that's what I set out to fix. This program distributes the cards somewhat regularly (while still keeping things a bit random) and it helps you build random decks.

# Main Window #

![http://ctislideshow.googlecode.com/files/MainWindow.jpg](http://ctislideshow.googlecode.com/files/MainWindow.jpg)

This is the main window that you see when you start the program. It's where all the action happens. To get started right away select **File -> New Slideshow**. You will be presented with the following:

![http://ctislideshow.googlecode.com/files/Setup1.jpg](http://ctislideshow.googlecode.com/files/Setup1.jpg)

All you do here is tell the program where your instruction card images are located. If you're organized and have them in a bunch of subdirectories you can select the top folder and check the **Recurse Subfolders** option.

![http://ctislideshow.googlecode.com/files/Setup2.jpg](http://ctislideshow.googlecode.com/files/Setup2.jpg)

If you've named your instruction cards a certain way, the program will automatically detect what they are. You can now tell the program to include any number of specific cards in the slideshow. Leaving a type at -1 will tell the program to choose from that type at random.

![http://ctislideshow.googlecode.com/files/Setup3.jpg](http://ctislideshow.googlecode.com/files/Setup3.jpg)

This is where you tell the program where your images folder is located and how many images you want in the slideshow. Like Step 1, you can have the program search subdirectories.

![http://ctislideshow.googlecode.com/files/Setup4.jpg](http://ctislideshow.googlecode.com/files/Setup4.jpg)

The last page! It's really just an overview of what you've set up so far, but you can also select how long each image is on screen for (remember: you can change this in-flight with the **+/-** keys). Once you click **Finish** the slideshow will begin.

# Slideshow Mode #

![http://ctislideshow.googlecode.com/files/Metadata.jpg](http://ctislideshow.googlecode.com/files/Metadata.jpg)

Once the slideshow starts, the main window displays the slideshow images. Along the top are three pieces of information:
  * (Left) Current image number / total images
  * (Middle) Image name
  * (Right) Image duration

If you've created [metadata](metadata.md) for your cards, you may see something happening on the right. Every time an instruction card is drawn and it has metadata, a little window on the right will appear with the metadata. This should help you keep track of which cards are in play and what instructions are in effect. If a card no longer needs to be displayed, there is an X button at the top right of each window. Click to close it.

There are some keyboard controls, too:
  * **Spacebar** Pauses/resumes the slideshow
  * **F11** Toggles between windowed and fullscreen mode
  * **Arrow Left / Right** Moves to the previous / next image
  * **+/-** Increases or decreases the image display time by one second
  * **Escape** Closes the window

# Metadata #

CTI Slideshow now has a metadata editor for your instruction cards. To open it select **Tools -> Card Metadata Editor**.

![http://ctislideshow.googlecode.com/files/CME.jpg](http://ctislideshow.googlecode.com/files/CME.jpg)

Point it at a folder that contains some instruction cards and you will see them listed on the left. In the middle is the image, and on the right are some textfields.

Here you're able to add some information about what the card is (the Title field, this is usually Stroke It! or whatever the card type is), what it does (the Description field), and what you need to use it (the Items Needed field, one item per line).

And that's pretty much it. If you take the time to add metadata to all your cards you'll see that information pop up in two places:
  * At the beginning of the slideshow you will be presented with a list of what you need to obey all instructions
  * During the slideshow, you'll see the metadata for each card appear at the right, if it exists. This should help you keep track of what cards are still in play. The X button will make the box go away.

At this point, you'll probably notice a bunch of .xml files in your instruction cards folder next to each image. **This is the metadata and please do not delete it** (unless you want to). Note that, even though the metadata contains the card's image file location, it isn't necessary. That means you can effectively move your cards and metadata wherever you want.

# Loading and Saving #

You can now load and save slideshow setups and complete slideshows. HOLY. SHIT.

**Slideshow Setups** are what you create when you run the New Slideshow wizard. It keeps track of your instruction cards folder, deck makeup, and image options but not the actual instruction cards or images used to make the slideshow.

Conveniently, you can quickly reload your most recent **Slideshow Setup** by selecting **File -> Load -> Load and Run Last Slideshow Setup**, or press **Ctrl+R**.

You can also save the most recent slideshow and reload it any time. All images and instruction cards will be reloaded.