# Links

# <https://linksinheaders.com>

That should not blow things up

# Text, Links, Lists and Tables

## LaTeX slashes should not blow us up

foo\bar is cool with me.

## Fonts and Text

Here is some formatted text: **bold** *italic*, `teletype`.

_italics_

__bold__

___bold and italic___

____underline____

*italics*

**bold**

***bold and italic***

****underline****

A right arrow => is cool.

and so is an -- en-dash.

These&nbsp;are&nbsp;non&nbsp;breaking&nbsp;spaces.

H~2~O is a liquid.  2^10^ is 1024.

It works by having a fully 360&deg; panoramic view, also showing separate windows for all participants.

These quotes should be "curly".

* This should be a curly apostrophe, shouldn't it?
* "I love curly quotes!", she squealed.
* And then … ellipses!
* emdash: —
* endash: –

## Code

and some code (the quotes should not be curly in the code):

With the language hard-set to Ruby:

{:lang="ruby"}
    #!/usr/bin/env ruby

    10.times do |n|
      puts "Hello, world '#{n}'!"
    end

hard-set with the new Leanpub directives syntax:

{lang=ruby}
    #!/usr/bin/env ruby

    10.times do |n|
      puts "Hello, world '#{n}'!"
    end

With language not set:

    #!/usr/bin/env ruby

    10.times do |n|
      puts "Hello, world '#{n}'!"
    end


This is a tilde delimited code block.

{lang=ruby}
~~~~~~~~~~~
#!/usr/bin/env ruby

10.times do |n|
  puts "I love tildes!"
end
~~~~~~~~~~~

{:lang="scheme"}
~~~~~~~~
foo
()
(foo)
(foo bar)
(a b (c) d)
~~~~~~~~

{:lang="scheme"}
    foo
    ()
    (foo)
    (foo bar)
    (a b (c) d)


This should not be highlighted:

{:lang="text"}
    Error: Something terrible has happened!
    at Timer.C (/AsyncJS/nestedErrors.js:4:13)

Inlined code:

<<(code/inline.rb)

Inlined Javascript:

<<(code/test.js)

Inlined code with a title:

<<[I has a title](code/inline.rb)

And again, with a more complex title:

<<[code/inline_with_underscores.rb](code/inline.rb)

Code wrapping

~~~~~~~~
#!/usr/bin/env ruby
# Long lines will be wrapped
puts "odd numbers from 1 to 100: " + 100.times.each.map {|number| number.odd? }.join(", ") + " are really odd, aren't they"
~~~~~~~~


### lists with code in them

* one

        #!/usr/bin/env ruby
        puts "hiya"
        10.times {|n| puts n}

* two
* three

### GitHub style codeblocks

Without any language setting:

```
def foo
  "foo"
end
```

With the language set to ruby:

```ruby
def foo
  "foo"
end
```

With the language set to text:

```text
def foo
  "foo"
end
```

### Adding and removing code

~~~~~~
#!/usr/bin/env ruby

def foo
  "Foo"
end

# leanpub-start-delete
def oldStuff
  "Old"
end
# leanpub-end-delete

# leanpub-start-insert
def newStuff
  "New"
end
# leanpub-end-insert

def normal
  "No change here"
end
~~~~~~
## Citations

There are also markdown style citations supported by Pandoc.

You need to provide a bibliographic database. See the Pandoc readme for more details.

Blah blah [see @doe99, pp. 33-35; also @smith04, ch. 1].

Blah blah [@doe99, pp. 33-35, 38-39 and *passim*].

Blah blah [@smith04; @doe99].

## Footnotes

You can write inline footnotes like this[^1]. You should probably use longer footnote names[^footnote].

Footnotes with URLs in them[^2] like this should not have footnote marks in the footnotes.

[^1]: this syntax originated in the PHP Markdown Extras package
[^2]: This has a link to <http://example.com> and [example](http://example.com).

































































[^footnote]: Numbering will happen automatically and have nothing to do with what you call a footnote. Also, Kramdown used to hang when you had a large number of newlines before a footnote definition, so that's why those spaces are there

## Links {#links}

A [link](http://example.com) which should show as a footnote below.

[**bold links**](http://example.com) should not blow up.

[links with tildes and pounds in them](http://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_2_1_1) should not replace tildes with nbsp and should not blow up on the # sign.

[links with # in them](http://example.com/foo.html#bar) should not blow up.

[links with % signs and ampersands in them](http://exmaple.com/%7dfoo.html?a=b&c=d) should not blow up.

[This should link to example.com/text][1]

A cross reference to [images](#images).

[foo | fie](http://example.com) (links with pipes in them should not blow up).

![hubspot refer developer $10k](images/hubspot_referdev_250px(web).jpg)] -- images with parens in their name should not blow up.

  * [** **](http://feeds.feedburner.com/ProductiveStrategy)**[Advanced Analog Integrated Circuits](http://webcast.berkeley.edu/course_details.php?seriesid=1906978506)** EE 240


A [reference link][2] to a link with quoted title

A [reference link][3] to a link with parentheses delimited title

A [link with square brackets [ ]][3] should not blow up.

A [*****](http://example.com) link with a bunch of stars in it.

A [link_with_underscores](http://example.com).

[http://feedproxy.google.com/r/OfficialHuitaleBlog/3/q\_19u5mfYog/single-product-owner-model-is-broken.html](http://feedproxy.google.com/r/OfficialHuitaleBlog/3/q_19u5mfYog/single-product-owner-model-is-broken.html)

### Badly formatted links

This link should not blow up book generation:

[this is a link with a quote a the beginning of the URL]("http://example.com)

### Russian Links

Links with Cyrillic characters used to be broken in PDFs and point to the local file system. These should open up on wikipedia.

[снифферских атак](https://ru.wikipedia.org/wiki/Анализатор_трафика)

[man-in-the-middle](https://ru.wikipedia.org/wiki/Атака_посредника)


## Lists

* This
* is
* unordered

Here's an ordered list:

1. one
2. two
3. three

You can also use roman numerals

i. one
ii. two
iii. three

or letters

a. is for apple
b. is for ball
c. is for cat

Lists with headers in the first item should just show the text as strong. Otherwise LaTeX blows up.

* ## Strong
* two

Nested lists

* one
  * two
    * three
      * four
        * five
          * six
            * seven

This list has a missing last item, and should not blow up:

* one
* two
* three
*

# Tables

## a simple table

{title="A sample table with some useful emails"}
| Name | email | Personal Website |
|---------------------------------------------------|
| Peter | peter@leanpub.com | http://peterarmstrong.com |
| Leanpub | hello@leanpub.com | https://leanpub.com |

## A multi-line table

{title="Figure 32: RESTful resources in S3"}
|Resource              |how it is constructed                     |GET                              |PUT                                  |DELETE                      |HEAD               |
|----------------------|------------------------------------------|---------------------------------|-------------------------------------|----------------------------|-------------------|
|Bucket                |  `/<bucket_name>`                        |Lists the bucket's objects       |Creates or updates the bucket        |Deletes the bucket          |N/A                |
|Object                |  `/<bucket_name>/`                       |Gets the object's contents       |Creates or updates the object        |Deletes the object          |Gets the object's  |
|                      |    `<object_key>`                        |                                 |                                     |                            |metadata           |
|ACL sub-resource      |  `/<bucket_name>?acl` or                 |Gets the ACL                     |Creates or updates the ACL           |N/A                         |N/A                |
|                      |  `/<bucket_name>/`                       |                                 |                                     |                            |                   |
|                      |  `<object_key>?acl`                      |                                 |                                     |                            |                   |
|logging sub-resource  |  `/<bucket_name>?logging`                |Gets the logging status          |Turns off logging for that bucket    |N/A                         |N/A                |
|                      |                                          |for the bucket                   |                                     |                            |                   |
|torrent sub-resource  |  `/<bucket_name>/`                       |Gets the BitTorrent `.torrent`   |N/A                                  |N/A                         |N/A                |
|                      |  `<object_key>?torrent`                  |file for the object              |                                     |                            |                   |




[1]: http://example.com/text
[2]: http://two.example.com "two"
[3]: http://three.example.com (three)

# Headers {#level1header}

Here is a new chapter!

## A Level 2 Header {#level2header}

Followed by a

### Level 3 Header {#level3header}

Followed by a

#### Level 4 Header {#level4header}

Followed by a

##### Level 5 Header {#level5header}

That's deep, ain't it!


## Paragraphs

Paragraphs will normally be nice and long and do you see any Teletubbies in here? Do you see a slender plastic tag clipped to my shirt with my name printed on it? Do you see a little Asian child with a blank expression on his face sitting outside on a mechanical helicopter that shakes when you put quarters in it? No? Well, that's what you see at a toy store. And you must think you're in a toy store, because you're here shopping for an infant named Jeb.

####

There should be a nice big fat space above this line


### Headers with [links](http://example.com)

should just show the text of the link

### Headers with images ![](images/25mic.jpg)

should not show the image

## Comments

The next line is a comment and should not show up in your book.

%% Psst. I'm a sneaky comment!
%%
%% And so am I!

This line is after the comment

This line has a hidden <!-- html comment -->html comment in it and an html comment after it

<!-- html comment -->



A cross-reference with [bad chars](#http://foo.com) in it should not blow us up.

A [link to just pound-sign](#) should not blow us up.
