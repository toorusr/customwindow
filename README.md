# CustomWindow ![](https://img.shields.io/badge/build-miserably--failed-red.svg)
> A script that uses windows as pixels and transforms these into one whole window.

I know, I know, I know, that sounds really insane and I do not want to deny that, but first I want to explain my motivation and my problem why this was developed.


## Story and idea
It all started with the fact that I absolutely wanted to have a shapeless window developed with python, because at that time I didn't know any other programming language. So I did a lot of research to find a solution, but there was nothing on the internet to start with at the time. So I tried to find a solution myself.

##### First idea
My first idea was actually to simply remove the native GUI buttons and use screenshots of the windows below as background of the window. With the help of items this window would have at least been rounded. But that wasn't really successful, since the computer performance simply doesn't play along with so many screenshots per second to maintain the transparency which was actually not available for this purpose. Also, there were just too many glitches on the screenshots, which in retrospect was probably due to the library I had used.

##### Second and last attempt
My last and second idea as well as the one where I lost motivation was to create a lot of windows where only the body could be seen and used as pixels. The moment I thought it would work out, I was thinking that everything would be great and I had almost reached my goal. However, I was wrong. The fact of creating 500 x 500 pixel windows alone, which in total would have been 250000 pixels, should have made me think it over. Unfortunately, this moment came rather late, but I learned from it. So I worked on my idea and implemented it. At some point I had noticed that when I create a lot of windows, even if they are very small, everything starts to jerk. After miserable attempts to eliminate this I gave up my great project.

##### Lesson
What have I learned from this?
So first of course to research more thoroughly and also to think more about the possible result, both I have done only quite roughly. I also learned a lot about python and experimented a lot.

## Result
Unfortunately I only have my second idea in code form and therefore I have only added this idea to this repository.
Nevertheless it doesn't work properly I want to explain how the script `CustomRoot.py` actually works.

##### Setup
1. Make sure you have python 3.x installed
2. Download the script [CustomRoot.py](https://raw.githubusercontent.com/toorusr/customwindow/master/CustomRoot.py)

##### Do something with it
Now here are two options
1. Figure it out by your self
2. Follow my constructions

```python
if persons_selection == 1:
    person.figureOut("CustomRoot.py")
elif persons_selection == 2:
    person.readAlong("README.md")
else:
    print("Why are you even doing this to your self?")
```
##### Trying to explain my own code
There is one function and one class that contains even more funtions.
The first function does what it is named like. The `center()` functions **should** center the window in the middle of the screen.
The class `CustomRoot` is pretty much the heart of the script and creates the CustomRoot.
Well, okay, to this point you should have kept up with me.
Now we will figure out together, because I don't actually remember at this point how the script works, how we can get something like a window out of this.

To do so we have my beautiful code and some comments. *Okay, I just have realised that I have not written any comments.*

At first to start the script we open up a terminal and type
```bash
python3 CustomRoot.py
```
My terminal just spit out `x1` and is now stuck in a loop.
The script created a window named `tk` with two buttons named `x++` and `y++`.
When I press them nothing happens, I think I wanted them to interact with the shape that has been generated.
Under the obscure window I found this shape out of ca. 900 pixels or how I called them in my code: 'winxels', what maybe win(dow pi)xel.

It seems like we can just inject pseudocode into the `root.shape()` function in line 120 after we created the root by initialising the CustomRoot class.
I will quickly test that by changing the argument that `shape()` takes.
```python
# line: 120
root.shape("x1y2x1y1")
```
On execution it gave me this error:
```
Traceback (most recent call last):
  File "CustomRoot.py", line 120, in <module>
    root.shape("x1y2x1y1")
TypeError: shape() missing 1 required positional argument: 'startpoint'
```
That means that the function shape takes two arguments.
I will quickly repeat what I did but with the startpoint coordinates, `(900,500)` added.

# License
This repository is licensed under the MIT License so you can do almost everything what you want with it.

See [LICENSE](https://github.com/toorusr/customwindow/tree/master/LICENSE).
