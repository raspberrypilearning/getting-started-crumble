## Button switches

The Crumble starter kit come with a great little Crumble friendly button switch but you could use any switch as long as you can connect to the switches terminals.

[Some switches](images/switch_selection.png)

Note: different switches work in different ways. We mostly think of switches as standard on/off switches but some are push to make (when you press them the switch is on but as soon as you stop pressing, the switch is off) and some are even push to break (on unless being pressed). The Crumble starter kit button switch is push to make.

All of the components that we have looked at so far have been outputs. The Crumble has sent information out to them and they have done something in response. The button switch is the opposite. It is an input which means something happens outside, i.e. someone presses the button switch, and the Crumble recieves that information. The switch is either on or off.

![inputs and outputs](images/inputoutput.png)

Let's connect up our switch.

--- task ---

First, let's connect positive power to the switch. Connect a croc clip from the positive (+) terminal of the Crumble at the top right corner to one side of the Crumble button switch (either side will do).

Next, we connect another croc clip from terminal A to the other side of the Crumble button switch. You could also use terminals B, C or D for switches.

![Connecting a button switch to your Crumble](images/switch_to_crumble.png)

--- /task ---

Now that it is connected, when the button is pressed terminal A is HI (on), and when the button is released terminal A is LO (off).

And now let's write some code.

--- task ---

As ever, we start with the `program start`{:class="crumblebasic"} block.

Next, we need to ask a question about what state the button is in. Is the button in its on or off state?

from the `control`{:class="crumblecontrol"} palette, grab the `if... then`{:class="crumblecontrol"} block.

![If... then block](images/if_then_block.png)

From the `Input/Output`{:class="crumbleinputoutput"} block palette, get an `A is HI`{:class="crumbleinputoutput"} block and place it inside the hexagonal space in the `if... then`{:class="crumblecontrol"} block.

--- no-print ---

![Inserting button blocks into IF statement blocks](images/AtoHI_in_if.gif)

--- /no-print ---

--- print-only ---

![Inserting button blocks into IF statement blocks](images/button_if_then_code_noForever.png)

--- /print-only ---

![Button switch code with no output](images/button_if_then_code_noOutput.png)

--- /task ---

Of course, we now need an output for the Crumble to be able to indicate the result of the input, or whether the switch is on or off.

You can use any input for this depending on your project, but for now, let's use a Crumble Sparkle.

--- task ---

Connect up a Crumble Sparkle as we did earlier in the project. Positive to positive, negative to negative and D to the D terminal of the Crumble. Rememmber that Sparkles only work with the D terminal! If you need a little more help, look **************************.

Now let's use our Crumble Sparkle output by adding some code.

Inside the conditional statement, add `set sparkle to *********`{:class="crumblesparkles"} from the `Sparkles`{:class="crumblesparkles"} palette.

![Button switch code with output](images/switch_code_with_output.png)

Now our code reads, when the `program starts`{:class="crumblebasic"}, `if`{:class="crumblecontrol"} `the switch is on`{:class="crumbleinputoutput"} `then`{:class="crumblecontrol"} `make sparkle light up *********`{:class="crumblesparkles"}. 

--- /task ---

At the moment, if the switch is off then the sparkle won't do anything because we have not told it to do anything. Let's fix that right away!

--- task ---

## Add a section to say else turn sparkle off

--- /task ---



