## Motors

The Crumble board is designed to be able to power two DC motors and when powered by 3 AA batteries the board outputs 4.5v to the motors.

You could use any simple standalone DC motor for this task, or a gear motor like the ones often used in making simple robot buggies. They all work the same and infact, inside the yellow casing of the gear motor shown, there is a simple DC motor just like the one on the right of the image.

![Three different DC motors](images/DC_motors.png)

Note: If you are using a 3v motor, running your motors at 70% the Crumble board will supply roughly the 3v output for which your motor was designed.

Most motors have clearly marked positive and negative terminals. If these are reversed it simply means that the motors will turn in the opposite direction.

--- task ---

The Crumble board's motor connections are the two terminals at the bottom end of the board on either side.

Connect one end of a crocodile clip the Motor 1 positive terminal (+). It is the second terminal up on the left side of the board. Connect the other end of the croc clip to the posive terminal of the DC motor. Again, this is usually marked with a '+' but if it is not clear which is the positive terminal, don't worry, just connect it to one of the two terminals.

Next, connect another croc clip from the Motor 1 negative terminal (-) to the negative terminal of the motor.

![Crumble to DC motor connections](images/motor_connections.png)

I have used red and black crocodile clips to make things clear, but any colours will work fine.

--- /task ---

Great! That's our motor connected up. Now to write our first motor controlling code!

--- task ---

As ever, let's grab a `program start`{:class="crumblebasic"} block to start our code.

Making the motor run is an output so let's look in the `Input/Output`{:class="crumbleinputoutput"} blocks palette for our motor control blocks. Can you see the one we need?

Grab the `motor 1 FORWARD at 75%`{:class="crumbleinputoutput"} block and connect it under the `program start`{:class="crumblebasic"} block.

Just so we don't have the motor jumping all over the table, let's change the power percentage to 25% to start with. Although jumping motors can be fun too!

![First Crumble DC motor code](images/Crumble_motor_forward_code.png)

Now click the green 'run' triangle to test your code.

--- no-print ---

![Running motor forward program](images/Crumble_motor_forward.gif)

--- /no-print ---

--- print-only ---

![Running motor forward program](images/Crumble_motor_forward.png)

When the 'run' button is pressed, the motor will spin. When the red 'stop' square is pressed the program ends and the motor will stop.

Tip: Sticking something on the end of the motor shaft makes it much easier to tell when the motor is spinning.

--- /print-only ---

--- /task ---

As we have seen, pressing the red 'stop' button will end the program and stop the motor but we can also stop the motor using code.

Clicking on the `FORWARD`{:class="crumbleinputoutput"} part of the `motor 1 FORWARD at 25%`{:class="crumbleinputoutput"} block will toggle between `FORWARD`{:class="crumbleinputoutput"}, `REVERSE`{:class="crumbleinputoutput"} and `STOP`{:class="crumbleinputoutput"}.
 
 --- no-print ---

![Toggle motor control](images/crumble_motor_direction_toggle.gif)

--- /no-print ---

--- print-only ---

![Toggle motor control](images/crumble_motor_direction_toggle.png)

--- /print-only ---

Now let's get a bit creative with our motor! Let's code a program that will tell the motor to go forward, then stop, go in reverse, then stop, and then repeat all of that three times.

--- task ---

Building on the program that we already have, grab a `wait 1.0 seconds`{:class="crumblecontrol"} block from the `Control`{:class="crumblecontrol"} blocks palette, and add it under the `motor 1 FORWARD at 25%`{:class="crumbleinputoutput"} block.

Get another `motor`{:class="crumbleinputoutput"} block and toggle the direction so it becomes a `motor 1 STOP`{:class="crumbleinputoutput"} block, and add it under the `wait`{:class="crumblecontrol"} block.

Next, we'll add another `wait`{:class="crumblecontrol"} block but this time get a `wait 100 milliseconds`{:class="crumblecontrol"} block, and connect under the `motor 1 STOP`{:class="crumbleinputoutput"} block.

Note: Since 1,000 milliseconds = 1 second, 100 millseconds is one tenth of a second. This means that a `wait 100 milliseconds`{:class="crumblecontrol"} block and a `wait 0.1 seconds`{:class="crumblecontrol"} block do exactly the same thing. Take your pick!

So that is the motor start and motor stop section. The next section is the same except going in reverse rather than forward. The quickest way to do this is to copy the blocks we have.

 --- no-print ---

![Duplicating code blocks](images/duplicate_blocks.gif)

--- /no-print ---

--- print-only ---

![Duplicating code blocks](images/duplicate_blocks.png)

--- /print-only ---

Right-click on the `motor 1 FORWARD at 25%`{:class="crumbleinputoutput"} block and choose 'Duplicate'. This copies that blocks and the three blocks below. Connect the blocks under the code you already have and toggle the `motor 1 FORWARD at 25%`{:class="crumbleinputoutput"} so it reads `motor 1 REVERSE at 25%`{:class="crumbleinputoutput"}.

Finally, get a `do 10 times`{:class="crumblecontrol"} loop block and put your code inside this (except the `program start`{:class="crumblebasic"} block which always starts our code, of course). Change the number of repeats from 10 to 3.

Your code should now look like this...

![motor control code](images/crumble_motor_start_stop_code.png)

Now, run your code and check that it does what you expect.

 --- no-print ---

![Motor running forward then reverse](images/crumble_motor_start_stop.gif)

--- /no-print ---

--- print-only ---

![Motor running forward then reverse](images/crumble_motor_start_stop.png)

The motor should run forwards, stop, reverse, stop, and repeat three times.

--- /print-only ---

--- /task ---