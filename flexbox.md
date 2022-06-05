# CSS3 Flexbox

![Flexbox](http://www.freewebtutorials.info/wp-content/uploads/css-flexbox.jpg)

___
##### Why Flexbox (Advantages)
___
- because its a CSS3 feature! LOL ... *seriously though*
- The flex(flexible) box module is meant to help lay out elements within applications.
- can be used very well to manage responsive websites.
- elements can be laid out in any flow direction (leftwards, rightwards, downwards, or even upwards!)
- easy to play around with the elements in the flexbox(changing the order and such)
- complex layouts can be achieved more simply and with cleaner code
- display order of the elements is independent of their order in the source code

With the old box model - Consider a scenario where we are creating a 4 column layout
```
.col {
    width: 25%;
    padding: 0 5%;
}
```
This would create 35% width instead (element width + padding) exceeding 100%. Usually we use `float` or `inline-block` to achieve the same in which case mostly we end up manually calculating the padding/margin values we need to provide to fit in the elements. These situations are avoided using the flexbox.

___
##### Flexbox Vocabulary
___
![Flexbox](https://mdn.mozillademos.org/files/3739/flex_terms.png)
- Flex container
- Flex item
- Main axis - axis along which the flex items follow each other.
- Cross axis - perpendicular to main axis.

Important properties to know
- `flex-direction` - establishes the main axis.
- `justify-content` - defines how flex items are laid out in main axis
- `align-items` - defines how flex items are laid out in cross axis.
- `align-self` - defines how a single flex item is laid out along the cross axis. Overrides its **align-items** value.
- `order` - Defines a value to a flex item which determines its ordinal position. Default is set to 0.
- `flex-wrap` - specifies if the flex items are forced into a single line or can be wrapped into multiple lines automatically. This is one of the main properties which is responsible for handling responsiveness using flexbox.
- `flex-flow` - shorthand combination for `flex-direction` & `flex-wrap`.

Advanced properties
- `flex-grow`
- `flex-shrink`
- `flex-basis`
- `flex` - shorthand combination of all the above advanced properties.

Note :: Properties like `float`, `clear`, `text-align`, `vertical-align` will have no effect on flex items.

___
##### Lets play!
___
What are we trying to achieve ?

![Codepen Demo](https://mdn.mozillademos.org/files/3760/HolyGrailLayout.png)

[link for the demo](http://codepen.io/PleaseBugMeNot/pen/EyJXJP)

___
##### Flexbox Playgrounds
___
- [Flexbox froggy](http://flexboxfroggy.com/)
- [Flexyboxes](http://the-echoplex.net/flexyboxes/)
- [Flexbox Demo](http://demo.agektmr.com/flexbox/)
- [Flexboxin5](http://flexboxin5.com/)

___
##### Good links to learn flexbox
___
- [Flex box properties](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [Flexbox Cheatsheet](http://www.sketchingwithcss.com/samplechapter/cheatsheet.html)
- [Tutorial site](http://flexbox.io/)

___
##### Browser Supports
___
IE9-, unfortunately, doesn't support flexbox at all. **IE10 supports the 2011 version**. [More on IE compatibility](https://msdn.microsoft.com/en-us/library/hh673531(v=vs.85).aspx)

**Opera 12.1+ supports the latest 2012 version** unprefixed. It will **also be supported by Chrome 30+ and IE11+**. **Firefox 22 already supports it**, too, but only partially — it doesn't support flex-wrap property and flex-flow shorthand.

Previous versions of Firefox, Chrome, and Safari 3.1+ support 2009 version. **Chrome 21+ also supports 2012 version** with prefix.

Also the [Can I Use reference](http://caniuse.com/#search=flexbox)

[Flexbugs](https://github.com/philipwalton/flexbugs#2-column-flex-items-set-to-align-itemscenter-overflow-their-container)
