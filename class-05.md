# Read 05 -HTML Images, CSS color & text

## Images
- add an image with ```<img>```, which is self-closing, or empty'

###```<img>``` attributes:
**src** source (usually a relative URL to iamges folder)
**alt** text description of image in case user can't see pic. Also for screen reader software.
  - if image is only for decoration and adds no content, use **alt** but leave " " empty
**title** extra info. Most browsers display as tooltip at hover
**height and weight** px. Specifying h&w helps browser load more quickly because it knows how much space to leave for images, which load more slowly.

### Placement
 -  if <img> is before a block element, the block element will start on new line below image
 - If just inside block element, the firtl row of text will start at bottom of image.
 - If inside block element, text will flow around image

 ### antiquated and previously used code 

 **align** attribute ```(``` left, right, top, middle, bottom ```)```


## 3 Rules for creating images
1. save in the right format ```(```jpeg, gif, png```)```
2. save at the right size- the same that it is to appear on websote
3. measure in pixels

**jpeg** is best when iamges has many different colors ```(photos)```
**gif** and **png** when images have few colors ```(```logos, icons...```)```

Resolution of an image is only important in print because screens determine the size of an image based solely on H&W in px

**GIFs** take a long time to load because they are composed of many frames and this makes the file size large

```<figure>``` element contains images and their captions. Can have multiple images in element, but they will all share the ```<figcaption>```

## Color
**color** is for text color
**background-color** default is transparent

use medium contrast. too little is hard for those with color-blindness or other visual impairments, too much is harsh on the eyes

**opacity** property specifies for element and child elements. Value is between 0.0 and 1.0

**rgba** property allows the choice of color and opacity. 'a' is alpha value 0.0-1.0

**HSL** colors are **hue** **saturation** and **lightness**
hue is angle
saturation is %
lightness is % ```(```0 is white, 100 is black```)```

## Text
**serif** has tiny stroke on each main stroke
**san serif** does not
**monspace** every letter is the same width

typeface will usually only display if it's installed on user's computer

**font-family** you can specify a list of fonts in case user's computer does not have font

**font-size** px, % (of default, which is 16), ems

**font-family** allows use of font;s URL that will be used in the event that font is not on user's computer
- fromat attribute 

**font-weight** bold or normal

**font-style** normal, italic, or oblique

**text-transform** upper- or lowercase or capitalize

**text-decoration** none, underline, overline, line-through, and blink```(```animates text to make it flash on and off ```)```

**leading** is the space between a letter's decender and ascender. **line-height** 

The vertical space between lines should be larger than the space between each word 1.4-1.5 em

**kerning** the space between each letter. use ems for 
**letter-spacing** and **word-spacing**

**text-align**
  - left 
  - right
  - center
  - justify - all lines , except last line, tales up full width of container

  **vertical-align** use with ```<img>``` ```<em>``` and ```<strong>```
values:
 - baseline
 - sub
 - super
 - top
 - text-top
 - middle
 - bottom
 - texxt-bottom
 can also take length in px or em 
 or % of line height

 **text-indent** indents first line of text in an element

