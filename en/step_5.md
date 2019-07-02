## Challenge: make your LED flash

Can you create code that makes your LED flash on and off?

--- no-print ---

![Flashing LED](images/flashing_LED.gif)

--- /no-print ---

--- print-only ---

![Flashing LED](images/flashing_LED.png)

--- /print-only ---

Think about what the LED is doing in each moment to flash. What instructions do you need to give the LED to make it flash?

--- hints ---

--- hint ---

This is what your program should tell the LED:

1. When the `program starts`{:class="crumblebasic"}, the LED `turns on`{:class="crumbleinputoutput"}

1. Then, `after half a second`{:class="crumblecontrol"}, the LED `turns off`{:class="crumbleinputoutput"}

1. Once the LED is off, `wait half a second`{:class="crumblecontrol"} again

So the LED keeps flashing on and off, all of that code needs to `repeat`{:class="crumblecontrol"} ten times (or however many times you like).

--- /hint ---

--- hint ---

In a repeat loop, after every block in the loop has run, the first block in the loop runs again, right after the final block in the loop.

Use the blocks below to create code to flash your LED.

![Crumble blocks needed for a flashing LED](images/flashing_LED_parsons.png)

Note: 1000 milliseconds make up one 1 second. So 500 millseconds is half a second. This means that a `wait 500 milliseconds`{:class="crumblecontrol"} block and a `wait 0.5 seconds`{:class="crumblecontrol"} block do exactly the same thing. Take your pick!

--- /hint ---

--- hint ---

You need a `wait`{:class="crumblecontrol"} block after every `on`{:class="crumbleinputoutput"} and every `off`{:class="crumbleinputoutput"} block.

Test the code below, and see if it does what you expect.

![flashing LED code solution](images/flashing_LED_code_solution.png)

--- /hint ---

--- /hints ---