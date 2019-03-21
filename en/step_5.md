## More Sparkle with RGB colour code

Now that we have one Sparkle working, let's add another one! This time we will use RGB (red, green and blue) values to set our Sparkle's colour.

--- task ---

Our second Sparkle will simply 'daisy chain' onto the first Sparkle. Where we attached croc clips going from the Crumble to the left hand side of the Sparkle, we will now do the same thing going from the right side of the first Sparkle tot he left side of the second Sparkle.

NOTE: Just like before, make sure that you connect positive to positve, negative to negative and signal (D) to signal (D).

![Wiring a second Sparkle](images/secondSparkleWire.jpg)

--- /task ---

Now we need to add some code to make the second Sparkle turn on.

--- task ---

In the Crumble software on your computer, we're going to try a new block from the Sparkle block palette.

Drag out the `set sparkle to`{:class="crumblesparkles"} block that ends with the three RGB value input boxes, `0`{:class="block3myblocks"} `0`{:class="block3operators"} `0`{:class="block3motion"} and connect it under your existing `set sparkle to`{:class="crumblesparkles"} block.

![Coding a second Sparkle](images/secondSparkleCodeBlocks.png)

--- /task ---

At the moment, both Sparkle blocks are set for `sparkle 0`{:class="crumblesparkles"}. 

The first Sparkle connected to the Crumble is given the name `sparkle 0`{:class="crumblesparkles"}, which slightly confusingly makes the second Sparkle, `sparkle 1`{:class="crumblesparkles"} and so on.

--- task ---

Set your second `set sparkle to`{:class="crumblesparkles"} block to control our second Sparkle, `sparkle 1`{:class="crumblesparkles"}, by clicking on the 0 inside the input box right after `set sparkle`{:class="crumblesparkles"}, inputting '1' and then pressing RETURN on the keyboard.

--- no-print ---

![Second Sparkle being set to Sparkle 1](images/secondSparkleSetTo1.gif)

--- /no-print ---

--- print-only ---

![Second Sparkle being set to Sparkle 1](images/secondSparkleSetTo1_noPrint.png)

--- /print-only ---

--- /task ---

### RGB colour mixing

Computers show colours by mxing different amounts of red, green and blue (RGB). Each  of these colours can have a value from 0 to 255, where 0 is no colour at all and 255 is the maximum. 

It is more like mixing light than mixing paint though, and you may be surprised by some of the colours that you get.

If all the RGB values are 0, you will get black. If all the values are 255, you will get white, but you can get millions of colours by combining the number in between!

--- no-print ---

![RGB colour mixing](images/RGBvalues.gif)

--- /no-print ---

--- print-only ---

![RGB colour mixing](images/RGBvalues_noPrint.png)

--- /print-only ---

Google have a neat little [RGB colour picker](https://www.google.com/search?q=color+picker){:target="_blank"} that you can use to explore different colour values.

[![Google's colour picker with RGB values](images/googleColourPicker.png)](https://www.google.com/search?q=color+picker){:target="_blank"}

Click on the [link](https://www.google.com/search?q=color+picker){:target="_blank"}, then click or drag the slider and colour space to find the colour of your choice. The RGB values will show to the left.

--- task ---

Enter a value in each or the `red`{:class="block3myblocks"}, `green`{:class="block3operators"} and `blue`{:class="block3motion"} input boxes in the `set sparkle to`{:class="crumblesparkles"} block.

![Set Sparkle to user defined RGB code](images/SparkleRGBcode.png)

Click the green 'play' triangle to run your code and see what colour combination you just created!

--- no-print ---

![Lighting your second Sparkle with RGB values](images/secondSparkleLights.gif)

--- /no-print ---

--- print-only ---

![Lighting your second Sparkle with RGB values](images/secondSparkleLights_noPrint.png)

--- /print-only ---

--- /task ---

The Crumble software does not give you any visual indication as to what your RGB value combination will produce but it's fun to experiment with different mixes. Predict what your combination will produce, run your code and see if you were right!

What colour do you think red:255, green:0 & blue:255 will give you?

What colour do you think red:255, green:255 & blue:0 will give you?

How would you combine red, green and blue values to get orange?

--- task ---

Play around wit the RGB values. 

Choose a colour and try and find the right values to make that colour, or choose the RBG values and try to predict what colour you will get.

A great game here is to use the `sparkle 0`{:class="crumblesparkles"} colour picker to choose a colour and then try and set the RGB values for `sparkle 1`{:class="crumblesparkles"} to get as close as you can. Challenge a code buddy!

Run your code to see if you were right each time!

--- /task ---