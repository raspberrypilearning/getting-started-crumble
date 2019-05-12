## Position servos

For this section you will need a servo and leads to connect your servo to the Crumble controller. Servos come with three wires ending in a female [type] socket. 

[A position servo](images/servo_example.png)

There are a number of ways that you could connect this to your Crumble. Here are three good options.

--- Use a Crumbliser to make things easy - see About Crumblisers below.
--- Use male to male jumper leads between the servo plug and crocodile clips.
--- Combine male jumper cables and crocodile clips to make a custom 'servo to Crumble' cable.

--- +++ About Crumblisers ingredient +++ ---

If you do not have the components needed, you can simply skip this section and the following challenge, and come back to them at any time. Missing this section and its challenge will not affect any of the sections that follow.

Unlike DC motors that simply turn at varying speeds, with position servos we send information telling the servo to go to a certain position. Most servos have a range of 0 to 180 degrees.

Note: While most servos are position servo, you also get identical looking servos called rotation servos that rotate in either direction in the same way that a DC motor does.

--- task ---

Connect your servo to your Crumble using the steps below according to what components you have available.

??? --- servo to Crumbliser to Crumble ---> ingredient ???
??? --- servo to jumper to croc to Crumble ---> ingredient ???
??? --- servo to hybrid jumper/croc to Crumble ---> ingredient ???

--- /task ---

Now we have the servo connected, lets code the servo to move.

--- task ---

Let's start with the `program start`{:class="crumblebasic"} block and add a `servo C 90 degrees`{:class="crumbleinputoutput"} block from the `Input/Output`{:class="crumbleinputoutput"} palette.

![Simple servo code](images/servo_to_90.png)

That's enough to get our servo to work in the most basic way. Click on the green 'play' button to move the servo to 90 degrees.

--- /task ---

Note: Make sure your code references the same terminal that you attached the signal cable to, e.g. if you connected your servo's signal wire (usually white or orange) to your Crumble's terminal B then your code block must say `servo B`{:class="crumbleinputoutput"}, otherwise that Crumble will not be talking to the servo!

Of course, if your servo was already in position 90 degrees, you will not see any movement. Let's add another position to our code to make sure we see some movement.

--- task ---

First, let's change the `90`{:class="crumbleinputoutput"} in our `servo C 90 degrees`{:class="crumbleinputoutput"} block to say `0`{:class="crumbleinputoutput"}.

Add another `servo C 90 degrees`{:class="crumbleinputoutput"} block to the bottom of your code, and change the `90`{:class="crumbleinputoutput"} to `180`{:class="crumbleinputoutput"}.

Of course the servo will need time to move between 0 and 180 degrees so we neeed to add a `wait`{:class="crumblecontrol"} block between the two `servo C position`{:class="crumbleinputoutput"} blocks. Let's make it a half second delay, or `wait 0.5 seconds`{:class="crumblecontrol"}.

![Two position servo code](images/servo_0_to_180.png)

Click on the green 'play' button to see you servo move to 0 degrees and then to 180 degrees positions.

--- no-print ---

![Servo movement](images/servo_movement.gif)

--- /no-print ---

--- print-only ---

![Servo movement](images/servo_movement.png)

--- /print-only ---


--- /task ---

