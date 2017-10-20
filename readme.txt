https://coolors.co/ for great color palletes.
https://tympanus.net/codrops/css_reference/ for css reference.
https://specificity.keegan.st/ - for checking css specificity value
https://fonts.google.com/ - for new fonts
https://caniuse.com/ - for cross browser checking
https://unicode-table.com/en/ - for value of unicodes in browser.
http://fontawesome.io/ - For awesome fonts
https://unsplash.com/ - For royalty free images.
http://publicdomainarchive.com/ - For royalty free images.
http://rgb.to/ - convert color to rgb values
http://nibbler.silktide.com/en_US - to test website design
https://website.grader.com/ - website grader

1 em = inherited font-size
1 rem = inherited from the root element , mostly the html tag.
font-weight : bold
font-style : italic
line-height : used to set height of text between two different lines.
Block elements : Height as content but take 100% width , always on new line. Eg .p tag
Inline : Height and width of content. 
To check if it is block or inline , add background color to it. 
width and height have no effect on the inline elements since they only take height and width of content.They need the display property to apply width or height to it.

You can change the behaviour by using display tag in the relevant css tag. 
display:block -> convert inline to block
display:inline-block -> properties of both inline and block.
display:none -> used to hide elements.
padding increases the size of the box model.Push elements from the edge of the container.
margin sets value outside of the box. Push other elements .
border adds a border between the padding and the margin of the element.
margin shorthand property follows border-width , style and color . Eg. 2px solid red.
If you apply padding to inline elements , it will only push the values vertically , not horizontally. You can increase the padding between top and bottom elements by specifying them as inline-block elements.
margin 0 auto - used to set it to center of the page.
max-width can be used for setting maximum value of the width. Use max width for responsive content.
If you find content overlapping the content , change display to inline-block.

If you don't want a specific element to not float , use the clear attribute in css.
Parent elements do not recognise the height of the floated element .
If all elements of a parent are floated , the parent itself will collapse. You can use overflow in the parent css to make it stay there. You can also use clearfix for the same purpose.
overflow : auto -> Adds a scrollbar.
For images , you should only set the width . Height will be automatically adjusted with the aspect ratio.
To make sure padding and border don't change the size of the box , use the box model fix.

To focus on a particular type attribute , use [type] inside square brackets. For eg. for targetting all type=search input boxes , use [type="search"] or to focus on just the type , use [type].
section > a is used to target only the child element . Not the descendent elements.
Sibling combinators -> h2 + p -> Only the p element after h2
h2 ~ p -> all p elements after h2. It targets all elements even if there is a another tag in between. for eg. if h2 p h1 p -> it will apply to all p as long as they are sibling.
p.classname -> to target all classnames with name classname inside the p tag.
.btn.cncl -> Only applies settings to classes having both btn and cncl class.

:first-child selects first child of element. Usually selects the first sibling. No need to mention the parent. Only works if it is the first child . If h1 is the first child , it doesn't apply it to the next p. For this you need to use first-of-type.
:last-child selects last child of the element. Usually selects the last sibling.

nth-child -> 
can use nth-child(odd/even) -> Usually used for displaying data in a table.
you can also use nth-child(number) -> To select a particular .
You can also use algebraic formula -> nth-child(an+b)

There is also nth-of-type as well.	

suppose you have an+b , b-> Start from which element. 
a-> Difference between first and second element. 

Suppose you need to start from 4th element , but you want to highlight 4th , 6th , 8th element , so your formula will be 2n+4
Better to use the child-of-type rather than just the child.

for before and after pseudo elements , you always require content attribute.
Suppose you need quotes before and after a statement , you can do this using the before and after pseudo selectors.

p * select everything inside a plate.

If you apply float to an inline element , the element will automatically becomes a block.

position element :
static -> default
inherit -> takes from parent.
relative -> you can send the values anywhere on the screen but inside the parent box.
absolute -> removed from the page flow. It starts flying on top of screen. It doesn't stay in the parent box , you can make it fly anywhere. It will stay on top of the screen. If you want to set absolute , then make the parent relative. Best use this approach if you want something to stay at a particular position on the screen.

While using position , float is ignored.
While using float , display is ignored. Try using backgroud color to check how everything stacks up.

To apply z index , you need to add relative position first. the elements which come first have higher z index.

n-th last child count from the back.

Media queries -> use to apply css if certain conditions are met.
It can also be included using @media in css.

Start with general selectors and go on ahead with specific ones.
You need to declare @font-face before you start using the font in the code
