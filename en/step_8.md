## Challenge: Follow me colour sequence

![Traffic light colours loop](images/challengeTrafficLoopBaseCode.png)

Using the code above, `sparkle 0`{:class="crumblesparkles"} will flash from red, to amber, to green, back to red and so on. `sparkle 1`{:class="crumblesparkles"} flashes the colour that was just on `sparkle 0`{:class="crumblesparkles"}.

--- no-print ---

![Traffic light colours loop running](images/challengeTrafficLoopBaseReal.gif)

--- /no-print ---

--- print-only ---

At the moment that `sparkle 0`{:class="crumblesparkles"} changes from red to amber, `sparkle 1`{:class="crumblesparkles"} will change to red. Then after half a second, `sparkle 0`{:class="crumblesparkles"} changes from amber to green, `sparkle 1`{:class="crumblesparkles"} as changes to amber. So `sparkle 0`{:class="crumblesparkles"} is always one step ahead of `sparkle 1`{:class="crumblesparkles"}.

--- /print-only ---

![Traffic light colours loop running](images/challengeTrafficLoopBaseReal.gif)

Can you rearrange the code and add any extra blocks if needed to make `sparkle 1`{:class="crumblesparkles"} show `sparkle 0's`{:class="crumblesparkles"} colour BEFORE it changes to the next colour in the sequence?

--- hints ---

--- hint ---

--- no-print ---

The finished code will look like this when you run it.

![Traffic light follow me loop running](images/challengeTrafficLoopSolutionReal.gif)

--- /no-print ---

--- print-only ---

In the old sequence, the colours changed at the same time, but in the new sequence, `sparkle 0`{:class="crumblesparkles"} and `sparkle 1`{:class="crumblesparkles"} will take it in turns to change colour.

The sequence will start with `sparkle 0`{:class="crumblesparkles"} being red, then `sparkle 1`{:class="crumblesparkles"} will also turn red. Next, `sparkle 0`{:class="crumblesparkles"} will change to amber followed shortly after by `sparkle 1`{:class="crumblesparkles"} also turning amber, and so on.

--- /print-only ---

Try and follow the colour sequence and note when each Sparkle changes to a new colour.

--- /hint ---

--- hint ---

The Sparkles never change at the same time so you will need to add extra `wait`{:class="crumblecontrol"} blocks to separate all the `set sparkle to`{:class="crumblesparkles"} blocks.

![Crumble wait block](images/CrumbleWait0.5Block.png)

You will also need to rearrange the `set sparkle 1 to`{:class="crumblesparkles"} blocks so that they match the `set sparkle 0 to`{:class="crumblesparkles"} blocks.

--- /hint ---

--- /hints ---