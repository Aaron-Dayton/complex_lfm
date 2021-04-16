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

This image has square brackets in its caption and is a gif:

![Hi, I am square []](images/gifimage.gif)

A reference style image in a reference style link to the image:

[![][26]][27]

This image has a few percent signs in the file name and is in a link:

[![][entrevista]][link]

This was a gif: ![](images/thisisagif.gif)

This image is bad **and** has a bad file name: ![](images/10.100.jpg)

This image does not exist: ![](images/doesnotexist.png)

An image with a path like `./images/thisisagif.gif`:

![](./images/thisisagif.gif)

An image with a backslash in it:

![](images\thisisagif.gif)

A missing image with a backslash in it:

![](images\foooooo.png)

A paragraph with nothing but an image inside an anchor tag:

[![](images/25mic.jpg)](http://example2.com)

An image with bold text in the caption:
