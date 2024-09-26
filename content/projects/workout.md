+++
title = "workout"
summary = "Long term toy project which I use to play around with Rust and WebAssembly but also  solves a real practical problem since my first marathon training cycle in 2016:  For complex running workouts: How long will my run take? What's the total distance?"
+++


During my first (and second) marathon training cycle 2016 I used the
[Jack Daniels](https://en.wikipedia.org/wiki/Jack_Daniels_(coach)) 
2Q training plans which are pretty much on on the complex side for individual workouts. 

Workouts such as `9.6E + 5 * (3 min I + 2 min jog) + 4 * (1min R + 2 min jog) + 3.2E`
are not only difficult to remember but it's actually pretty difficult to judge the overall duration and 
overall distance. 

Since I was playing around with the Rust programming language at this time I started a
[CLI tool]("https://github.com/bernh/workout") able to parse the workout syntax and calculate total time
and distance.

This was 2016, just a couple of months after Rust 1.0 was released. I have maintained the code over the
years (including updating Rust versions, dependencies and rewriting the parsing code 3 times). 
8 years later I also wrote a simple GUI that is embedded on this page 
(with [egui](https://github.com/emilk/egui), all code compiled to WASM).

