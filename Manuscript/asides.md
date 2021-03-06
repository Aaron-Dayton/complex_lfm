# Asides, Tips and Warnings

> ## Blockquotes
>
> A blockquote should be indented.
>
> The second paragraph should be indented as well.
>
> And the third!

## Nested Blockquotes

> > > > > > > > Should not blow up.

A> ## Asides
A>
A> This is an aside.
A>
A> This is also sometimes known as a sidebar.
A>
A> To make one of these, put `A>` at the beginning of the lines of the aside, similar to the `>` that you use for a blockquote in Markdown.

E> ## ERROR!
E>
E> Warning, Will Robinson, Error!
E>
E> These, we have in abundant supply:
E>
E> src/Text/Pandoc/Readers/Markdown.hs:319:22:
E>
E> Couldn't match expected type `Text.Parsec.Prim.ParsecT
E>
E> In the expression: error
E>
E> In the expression: [codeBlockDelimited, ...]
E>
E> In the first argument of `choice', namely
E>
E>   `(if stateStrict st then
E>
E>         [header, codeBlockIndented, blockQuote, aside, ....]
E>
E>     else
E>
E>         [codeBlockDelimited, macro, header, table, ....])'

I> ## Information
I>
I> For your information, the following changes have been made:
I>
I> Information has been added.
I>
I> That is all.

Q> ## Question?
Q> 
Q> How much would you pay for this book?

T> ## Tips
T>
T> To make a tip, put `T>` at the beginning of the lines of the tip, similar to the `>` that you use for a blockquote in Markdown.
T>
T> To make paragraphs in a tip, you need to put lines with just `T>` between your paragraphs.

W> ## Warning!
W>
W> Warnings are generated by using `W>` at the beginning of lines.

D> ## Discussions
D>
D> Talk amongst yourselves. I'm feeling a little verklempt.
D> 
D> Well, the way they make shows is, they make one show. That show's called a pilot. Then they show that show to the people who make shows, and on the strength of that one show they decide if they're going to make more shows. Some pilots get picked and become television programs. Some don't, become nothing. She starred in one of the ones that became nothing.
D> 
D> The path of the righteous man is beset on all sides by the iniquities of the selfish and the tyranny of evil men. Blessed is he who, in the name of charity and good will, shepherds the weak through the valley of darkness, for he is truly his brother's keeper and the finder of lost children. And I will strike down upon thee with great vengeance and furious anger those who would attempt to poison and destroy My brothers. And you will know My name is the Lord when I lay My vengeance upon thee.

X> ## Exercises
X>
X> Do 3 sets of this every other day:
X>
X> * 20 squats
X> * 20 push-ups
X> * 20 standing lunges
X> * Plank for 20 seconds
X> * 10 pull-ups
X> * 30 jumping jacks

{icon=automobile}
X> # Custom
X>
X> I have a custom icon! Vroom!

{icon=doesnotexist}
X> # Nonexistent Custom
X>
X> I have a custom icon that does not exist.
X>
X> I should not blow up and should just show a warning icon.
