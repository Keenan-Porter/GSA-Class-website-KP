The general idea for this project was to first implement a boids simulation. The second idea was to use audio as an input for the project. I started by completing the tutorials for boids, and I integrated audio input into the project.

I had a few issues implementing boids. I struggled to sort out correctly defining and buffering the agents. I wanted to add more agents but I ended up hitting the buffer limit at about 60k on my laptop. I then had some small issues where I was defining certain things in my main.js, I had just put this into the script without thinking about when things needed to be defined. Overall, it wasn’t a difficult process and mostly went off without a hitch.

I struggled to implement audio input despite the simple process because of some issues with my browser. Otherwise, the implementation was pretty easy. I attached the mid range of audio to the distance the boids keep away from each other, which means they scatter when there’s a lot of noise. I made the highs affect the speed limit of the boids which mean at higher pitched values the boids move faster. I think this was an okay way of implementing it at first but the mid range audio has the highest values so it causes a lot of panic and breaks the simulation slightly. The high range has a much smaller effect making the speed difference not as visible.

When swapping the effects of the high and mid range, it created a much more chaotic result. I would compare it to a hurricane or tornado of triangles violently flying around the screen. To make it a bit more manageable, I reduced the multiplier that affects the speed limit so that.

Additionally, a modification I made from the original design is that the boids will be moved when moving beyond the screen to the opposite side, creating an infinite scrolling effect. This causes a lot of interesting behavior since sections of the boids will be thrown wildly off to another part of the screen. This also breaks the simulation slightly as it “loses” boids over a period of time. I’m not sure what is happening, but the number of boids is visually reduced when put into a lot of chaos.

I really enjoy the effect that is created by this project, it acts like some nexus type structure around the center of the screen.

My original intent for this was to try and mimic a normal flock of birds when a loud noise goes off. When it's quiet, the boids all just normally wrap around each other. But, when there’s loud noise the boids go crazy. With steady noise, the boids move around a bit more consistently being nudged in certain directions by sounds.
