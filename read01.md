# Viewport Units

> Viewport units are an interesting and *relatively* new method of defining length values for elements based off the size of a viewport itself. These units are used in the context of responsive web design by dynamically assigning length values for any CSS attribute that will accept them. Some of these attributes include: border-width, margin, font-size, padding, height, or grid-templates. This list is by no means exhaustive but hopefully demonstrates the versatility of viewport units. 

#### Viewport Width (vw): 
This unit by default represents 1% of the total viewport width. When prefaced with an integer it takes that percentage instead. E.g. 63vw will define a length value for the defined CSS attribute as 63% of the total viewport width. 

#### Viewport Height (vh): 
This unit by default represents 1% of the total viewport height. When prefaced with an integer it takes that percentage instead. E.g. 24vw will define a length value for the defined CSS attribute as 24% of the total viewport width. 

#### Viewport Minimum (vmin) and Viewport Maximum (vmax):
 These units work similarly to vw and vh as defined above. However, they first evaluate which value (of the viewport’s height and width) is smaller or larger and then reference that value. These units can be very useful tools when implementing different styling for portrait or landscape orientations. 

##Further Reading: 

[MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/length)

[Check if viewport units are compatible with the browser version(s) for which you are designing.](https://caniuse.com/#feat=viewport-units)