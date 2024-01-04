+++
title = "workout"
summary = "Long term toy project which I use to play around with Rust and WebAssembly but also  solves a real practical problem since my first marathon training cycle in 2016:  For complex running workouts: How long will my run take? What's the total distance?"
+++


During my first (and second) marathon training cycle 2016 I used Jack Daniels 2Q training plans 
is a bit on the complex side for individual workouts. 

Workouts such as `9.6E + 5 * (3 min I + 2 min jog) + 4 * (1min R + 2 min jog) + 3.2E`
or  `45 min E + 2 * (3.2T + 2 min rest) + 1.6T + 1.6E` are not only difficult to remember
but it's actually pretty difficult to judge the overall duration and overall distance. 

Since I was playing around with the Rust programming language at this time I started a
[parser]("https://github.com/bernh/workout") for the workout syntax with the final goal
of generating *fit* files compatible with my Garmin running watch. (The fit files describes the
workout steps and your watch then guides you thorugh the different steps)

Life got into the way and I never managed to actually implement the generation of the fit files
but I implemented at least the parser and the calculation of overall duration and distance which was 
also useful.

Over the years, whenever I had the urge to dust off my Rust I came back to this project. This typically
included making it work with new Rust versions, updating to new versions of dependencies, doing cosmetic
changes, etc.

In 2023 it was time to try Web Assembly and can see the results here: Some very primitive HTML and javascript
using the Rust implementation via Wasm. 

