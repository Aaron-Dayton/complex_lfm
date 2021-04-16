# Images {#images}

[This should link to example.com/images][1]

this image leaks out of the page as inline images are not properly supported: ![](images/at.png)

this image is just fine and has a caption:

![Oh, how I miss the 70s](images/25mic.jpg)

This image has a caption with an auto-link in it:

![<http://example.com>](images/smile.png)

This is an image with no src:

![]()

This is an image with no src, but with a caption:

![Some caption]()

This image has a filename including `.`s: ![](images/bad.file.name.png)

Here's an image within a nested subdirectory:

![](images/nested/smile2.png)

This image has a bad file name and is a gif, so needs to be converted:

![](images/811.strip.gif)