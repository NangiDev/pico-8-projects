# pico-8-projects

Work in progess!

Feel free to use everything as you please. Some creds would be fun, but not mandatory.
The graphics for Ninja.p8 are all made by me, but are heavily inspired by another game, Super Crate Box http://supercratebox.com/

Also a good site I would recommend are https://github.com/clowerweb/Lib-Pico8.

I can't take all the cred though!

Some stuff are more or less done, but I need to sort and clean some stuff.
Will probably create like a WIP folder and have "games" and "tech" as done-folder.

# Games

 Ninja                 |   JetPac                |   Corrupted Scrapyard
:---------------------:|:-----------------------:|:-----------------------:|
![./gifs/ninja.gif](./gifs/ninja.gif?raw=true "Ninja")  | ![./gifs/jetpac.gif](./gifs/jetpac.gif?raw=true "JetPac") | ![./gifs/scrappy.gif](./gifs/scrappy.gif?raw=true "Scrappy")
[My ninja game](./games/ninja.p8) | [My JetPac game](./games/jetpac.p8) | [My scrappy game](./games/crupt_scrpyrd.p8)
More or less done. Needs a end game. It is heavily inspired by Super Crate Box | JetPac is done. It's a clone of the old JetPac that developed for the ZX Spectrum. It was developed for the Banana Jam that Indie Gothenburg hosted. | Scrappy is not even playable. I had an idea, but it sort of spiraled away and became lots of tech demos instead.

# Tech

 Shadow Test           |   Bastion                |   Animation
:---------------------:|:-----------------------:|:-----------------------:|
![./gifs/shadow.gif](./gifs/shadow.gif?raw=true "Shadow")  |                                                                 ![./gifs/bastion.gif](./gifs/bastion.gif?raw=true "Bastion") |                                                               ![./gifs/animation.gif](./gifs/anim.gif?raw=true "Animation")
[Real time shadow](./tech/shadow_test.p8) | [Bastion inspired plattforms](./tech/bastion.p8) | [Animation loop](./tech/animation.p8)
I wanted to implement a shadow cast algorithm. It ended up okay, but as you can see there are some seperations between the shadows. Will maybe fix in future ;) | Bastion, made by Super Giant Games, are one of my favorite games and I really like theirs implementation of the plattforms appearing as you progress into the game. This is my implementation on that. | Just an animation loop I took from https://github.com/clowerweb/Lib-Pico8 and modified to fit my games better. Thank you guys!

 Bitwise wall detection |   Rolling ball                |   jump and fall
:---------------------:|:-----------------------:|:-----------------------:|
![./gifs/bit_shadow.gif](./gifs/bit_shadow.gif?raw=true "Bit shadow")  |                                                           ![./gifs/rollball.gif](./gifs/rollball.gif?raw=true "Rolling ball") |                                                         ![./gifs/jumpfall.gif](./gifs/jumpfall.gif?raw=true "Jump and fall")
[Detect wall facing](./tech/bitwise.p8) | [Ball in slope](./tech/rolling_ball.p8) | [Jump and fall test](./tech/jump_fall.p8)
This is basically the same as Shadow Test, but with only the walls facing the player in concideration. I used a bitwise technique to determine active wall. It contains a mayor memory leak that I have not yet found! | WIP! This is suppose to be a ball roling down slopes. My plan is to use graham scan on the map to generate the map with slopes and then make the ball roll down the slopes to the bottom of the screen. | Just a simple jump and fall implementation with animation. As of now the player can fly by holding down the jump button. Maybe not ideal! :) 

 Graham Scan           |   Push Objects                |   Linear Interpolation
:---------------------:|:-----------------------:|:-----------------------:|
![./gifs/graham.gif](./gifs/graham.gif?raw=true "Graham")  |                                                                 ![./gifs/pushObj.gif](./gifs/pushObj.gif?raw=true "Push Objects") |                                                           ![./gifs/lerp.gif](./gifs/lerp.gif?raw=true "Linear Interpolation")
[Graham Scan](./tech/graham_scan.p8) | [Push some objects](./tech/push_obs.p8) | [Linear Interpolation](./tech/lerp.p8)
This is the graham scan I am planing to use in the Rolling Ball implementation. It is defenetly not finished as you can see on the gif, but atleast I have started of in the right end. I think xD | Started of as a test to inherit position and to the object above the lower one. Now it is almost a game! I have plans on making this into a game where you compete with a friend on who is faster filling in holes. |Just a simple linear interpolation test I did. Steer the cube with the arrows and watch it interpolate its way towards that direction!

 Flag test           |   List sort                |   Polyfill
:---------------------:|:-----------------------:|:-----------------------:|
![./gifs/flag.gif](./gifs/flag.gif?raw=true "Flag test")  |                                                                   ![./gifs/sort.gif](./gifs/sort.gif?raw=true "List Sort") |                                                                   ![./gifs/polyfill.gif](./gifs/polyfill.gif?raw=true "Polyfill")
[Flag test](./tech/flag_test.p8) | [Sort a list](./tech/sort_list.p8) | [Polyfill](./tech/polyfill.p8)
Simple flagtest. Each color on the cube represent a flag toggled on or off. Use the keys to choose which one to toogle!| I needed a way to sort a list. This was a simple example I found in the pico-8 forums somewhere. There should be some more efficient way to do this. In some of my implementations this sort function is the one causing performance issues. I think! | Pico-8 can only draw lines, rectangles and circles as geometries. So I made a polygon filler. I use this in all my shadow implementations. It could probably need some performance improvments!

 Weapon system           |   Bitwise wall type   |   More to come!
:---------------------:|:-----------------------:|:-----------------------:|
![./gifs/weapon.gif](./gifs/weapon.gif?raw=true "Weapon System")  |                                                           ![./gifs/bit_wall.gif](./gifs/bit_wall.gif?raw=true "Bastion") |                                                             ![https://www.lexaloffle.com/gfx/lexaloffle-pico8.png](https://www.lexaloffle.com/gfx/lexaloffle-pico8.png?raw=true "PIco-8 logo")
[A weapon system](./tech/weapon_sys.p8) | [Bitwise wall type detection](./tech/bitvise.p8) | [Pico-8!](https://www.lexaloffle.com/pico-8.php)
This is the weapon system I use in my Ninja game. It is more like a mockup just to get a better view of what I wanted to do.  | Bits are a nice way to determine what type of wall each tile is. Every number represent the state of the wall. | I dont have anymore to show right now, but there are tons of cool stuff on pico-8's website. Check it out!
