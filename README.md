#Interview Question
[http://process-smith.com/frog.html](Live demo)
---
>You are a frog and you are trying to get across a river, in front of you are a series of lilly pads and gaps.
>If you land on a lilly pad, you are safe, if you land on a gap, it's sad.

>You can jump to N, N+1, or N-1 spaces in front of you, where N is your current velocity. Your starting velocity is 0.
>Velocity = the previous number of spaces you jumped.

>For example: here is a representation of what you see in front of you: [true, false, true, true, false, true, true, true]
>true indicates there is a pad, false indicates there is a gap. 

>Write a function that takes as input, an array like above and outputs the fastest safe route across the river, and returns false if it is impossible to get across.
>Example output: [1,2,3,3], [1,2,3,4] both get you across the fastest in the example input.
>Your goal is to get past the end of the array, so any space past the last one is safe.

##Solution
---
I created a tree of all possible outcomes and then traverse the tree to find the shortest path.
