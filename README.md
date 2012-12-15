Bot Pong and a Midnight Eureka
=======

This project was for CS490 class. You can view the recap of the competition on [youtube](http://example.net/).

Everything is built on the [HandyBoard](http://handyboard.com/hb/) (Built on the motorola 68HCxx), and using a lego robotics kit.

The Hardware
----------
Our hardware design was almost an accident. We knew we wanted to be able to "hold" all the balls on the field, as a gray area in the rules never said that you couldn't capture all the balls and simply drive to the other side of the court.

Other ideas that our prof shot down in fairness was no IR remotes, and no additional investments in hardware beyond $40 (So no tilt sensors or compasses).

Then my partner stumbled across the brilliant independent flexing arms, which ended up making our turns smooth, balls in a corner a non-problem, and the sturdiness of the design allowed us to travel easily twice as fast as any other competitors.

You can never downplay the importance of solid hardware, and given our superior hardware, our software had a platform to flourish on.


The Concept
----------
Our intital coding was similar to the rest of what we had done throughout the course. See the CompeitionInitial.ic. The way we looked at it was simply to drive around in a rectangle, and essentially hope that we didn't get to stuck or far off track. The code was organize spaghetti. If and else statements litered throughout, tracking and counter variables. Inefficient while loops.

While this worked [flawlessly](www.youtube.com) and we were fairly happy with it, on a late night a couple days before the competition it struck me that we could use the concept of a finite state machine to build an even better bot. (This also lead me to another [realization about my degree](http://blog.jaredshort.com/post/37952932982/why-a-computer-science-degree-matters)) We were able to throw together a much more sophisticated bot in only a couple hours. Checkout CompetitionUsingFSM.ic, it's pretty understandable, and efficient. Considering we had only two light sensor and two touch sensors it behaved better than we could have ever expected. Note that Interactive C as a language doesn't have a lot of the normal control-flow or features that modern languages support So no switch statement which would have been nice to clean up the code a bit more. We also made heavy use of constants and macros to build nice code.

The Conclusion
------------
This was one of my favorite classes to have participated in, and I am really excited to throw it up in hopes that someone else can get creative insight into problem that they are or will be working on.



Code
------------
Feel free to use or modify this code for any purpose.

*If someone else can figure out a quick or better unstuck routine I'd love to hear how you did it.