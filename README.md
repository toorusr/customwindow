# CustomWindow ![](https://img.shields.io/badge/build-miserably--failed-red.svg)
> A script that uses windows as pixels and transforms these into one whole window.

I know, I know, I know, that sounds really insane and I do not want to deny that, but first I want to explain my motivation and my problem why this was developed.


## Story and idea
It all started with the fact that I absolutely wanted to have a shapeless window developed with python, because at that time I didn't know any other programming language. So I did a lot of research to find a solution, but there was nothing on the internet to start with at the time. So I tried to find a solution myself.

##### First idea
My first idea was actually to simply remove the native GUI buttons and use screenshots of the windows below as background of the window. With the help of items this window would have at least been rounded. But that wasn't really successful, since the computer performance simply doesn't play along with so many screenshots per second to maintain the transparency which was actually not available for this purpose. Also, there were just too many glitches on the screenshots, which in retrospect was probably due to the library I had used.

##### Second and last attempt
My last and second idea as well as the one where I lost motivation was to create a lot of windows where only the body could be seen and used as pixels. The moment I thought it would work out, I was thinking that everything would be great and I had almost reached my goal. However, I was wrong. The fact of creating 500 x 500 pixel windows alone, which in total would have been 250000 pixels, should have made me think it over. Unfortunately, this moment came rather late, but I learned from it. So I worked on my idea and implemented it. At some point I had noticed that when I create a lot of windows, even if they are very small, everything starts to jerk. After miserable attempts to eliminate this I gave up my great project.

##### Lektion
What have I learned from this?
So first of course to research more thoroughly and also to think more about the possible result, both I have done only quite roughly. I also learned a lot about python and experimented a lot.

## Result
Unfortunately I only have my second idea in code form and therefore I have only added this idea to this repository.
Nevertheless it doesn't work properly I want to explain how the script `CustomRoot.py` actually works.

###### Setup
1. Make sure you have python 3.x installed
2. Download the script CustomRoot.py

###### To something with it
(I am currently editing this part)
