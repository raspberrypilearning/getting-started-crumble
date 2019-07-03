## Use servo motors with your Crumble

**Note:** If you do not have the components listed here, skip this section and the following one. Skipping these sections doesn't affect any of the sections that follow.

For this section you need:
* A servo motor, which usually has three cables ending in a single 'male' plug
* Either some male-to-male jumper cables
* Or a Crumbliser connector (shown below)

![Some position servos](images/servo_example.png)

![Jumper cable and Crumbliser](images/jumper.png)

You can turn DC motors like the one in the previous section at varying speeds. But you can tell position servo motors to rotate to specific positions.

While most servo motors are position servo motors, there are also rotation servo motors that look almost the same. Rotation servos rotate in either direction in the same way that a DC motor does.

Most position servo motors have a rotation range of 0° to 180°. The Crumble software uses this range as -90° to 90°.

--- task ---

Connect your servo motor to your Crumble using the steps below.

[[[servo-to-crumble-using-crumblisers]]]
[[[servo-to-crumble-using-jumper-cables]]]

--- /task ---

Now the servo is connected, create code to tell the servo to move.

--- task ---

* As always, start with the `program start`{:class="crumblebasic"} block.
* Click on the `Input/Output`{:class="crumbleinputoutput"} blocks menu, and drag out a `servo A 0 degrees`{:class="crumbleinputoutput"} block.
* Add the `servo A 0 degrees`{:class="crumbleinputoutput"} block below your the `program start`{:class="crumblebasic"} block

![Simple servo code](images/servo_code_to_0.png)

**Note:** Your code needs to include the name of the terminal that the motor is connected to. So if your servo's signal cable (usually white or orange) connects to your Crumble's terminal A, then your code block must say `servo A`{:class="crumbleinputoutput"}, so your Crumble can't talk to the servo!

* Click on the green triangle **play** button to move the servo motor to 0 degrees. 0 degrees is right in the middle of the servo motor's range.

If your servo is already at 0 degrees, it will not move.

--- no-print ---

![Servo movement](images/servo_movement_0.gif)

--- /no-print ---

--- print-only ---

![Servo movement](images/servo_movement_0b.png)

--- /print-only ---

--- /task ---

 Add another position to your code to make sure you see some movement.

--- task ---

* First, change the `0`{:class="crumbleinputoutput"} of your `servo A 0 degrees`{:class="crumbleinputoutput"} block to `-90`{:class="crumbleinputoutput"}.

You need to give the servo time to move to a different position.

* Add a `wait`{:class="crumblecontrol"} block below the `servo A position`{:class="crumbleinputoutput"} block. Make to motor wait for one second, so have the block say `wait 1.0 seconds`{:class="crumblecontrol"}.

* Add another `servo A 0 degrees`{:class="crumbleinputoutput"} block to the bottom of your code, and change the `0`{:class="crumbleinputoutput"} to `90`{:class="crumbleinputoutput"}.

![Two position servo code](images/servo_code_-90_to_90.png)

* Click on the green triangle **play** button to run your code.

The servo should move move 180°.

--- no-print ---

![Servo movement](images/servo_movement_-90_90.gif)

--- /no-print ---

--- print-only ---

![Servo movement](images/servo_movement_-90_90b.png)

--- /print-only ---


--- /task ---

