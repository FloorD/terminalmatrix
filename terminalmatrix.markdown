###Terminal Matrix

Today we'll teach you some tips and trics on how to use the terminal (or: command prompt) to make it appear to non-developer bystanders like you're in the matrix. The terminal is more than a place where you enter commands to your computer. You can count how often a word appears in a single file, pull a random Chuck Norris quote using the [Chuck Norris API][1], post a tweet from there or convert a large number of pictures to thumbnails. Just to name a few things. Plus: you don't need to install anything, as every computer has such a terminal thing. Let's get started:  
Python is already in your terminal. WHAT? How did that happen? Well, Linux and Mac operating systems come with Python already installed, so you can run it from the terminal simply by typing ```python``` (this is called the 'interactive mode'):

``` 
1 + 1  
```

There you have it, the basicest (is that even a word?) of math works in your terminal. Hit the + and everyone lurking by your computer will think you're an evil hacker! Consider using python in your terminal, the next time you need to calculate something!  

Another example of python's interactive mode, just to get the flow of things? Type (line by line!):  

```
the_world_is_flat = 1  
if the_world_is_flat:  
    print("Be careful not to fall off!") # don't forget to indent this sentence with 4 spaces, it's a python thing...  
```

See that #-thing? That means that whatever follows is a comment. You should not copy these and paste them in your terminal. Not that something bad will happen, but nothing much will happen! 
Use ```Ctrl-D``` to exit the interactive python 'shell'.

#####Hello, PyLadies! 

Standard practice when learning a new language is writing a little ```Hello, World!``` program. This is also where a texteditor comes in. Now there are a lot of different texteditors out there (developers can be picky people), but you want to download [Sublime][2] today as it's a free solution and quite an industry standard.  
What about that ```Hello, World``` huh? Open your text editor and write:  

```print("Hello, World!")```

Save the file, and name it "hello.py". Open the terminal (or console, in Windows, by clicking Start->Run and typing "cmd" into the prompt) navigate to the directory where you created your first program. Directory-WHAT? Yep, you can use your terminal to create folders on your computer. And folders in folders. And files in folders. And you can switch in a folder, much like you would just open something in your finder. But then cooler. How? 

```
mkdir PyLadies # make a directory and call it PyLadies
cd PyLadies # change the directory to the PyLadies one, so I can work from there
mkdir Images
mkdir Files
```
Typing in ```open .``` will open the whole directory for you, where you'll find your Images folder and you Files folder. 

Moving back to your ```hello.py``` file, make sure it's saved in your Files folder and switch to your Files folder using the terminal:  

```cd Files```

Now, type ```python hello.py```. Your terminal will (if all went well) return the following:

```Hello, World!```  

... and you're ready for the cool stuff! 

#####Some weird-arsed shit
Python lets you use single quotes AND double quotes, although not interchangeably (if you start with one, you have to end with the same one). Python also has a two more types of quotes. A triple quote, ''', is created by typing three single quotes. A triple-double quote, """, is created by typing three double quotes. So, you can have several layers of quoting before you need to worry about escaping your quotes. For example, this is valid Python:

```print """I wish that I'd never heard him say, '''She said, "He said, 'Give me five dollars'"'''"""```

#####Turtle shell

Another funny thing of the Python interactive shell is [Turtle Shell][3]. We'll be moving a (imaginary) turtle on a screen. To start type:  

```
python
import turtle
turtle.forward(15)
```

Repeat that last command (```turtle.forward(15)```) a few times an you'll see our turtle moving 15 pixels in the direction it is facing, drawing a line as it moves.  Up for a roadtrip?  

```
turtle.right(25) # rotates in-place 25 degrees clockwise
turtle.backward(10)
turtle.color("green") # makes the arrow green  
turtle.pencolor("green") # makes the line green
turtle.showturtle() # or: turtle.st(), to make sure the turtle is visible
turtle.shape("turtle") # to give the turtle it's turtle-shape (alternatively: turtle.shape("circle"))
turtle.shapesize(5, 5, 12) # makes it a rather big turtle
turtle.reset() # to go back to the middle of the document and erase all lines
```

Try and draw the first letter of you name (find more hints [here][4]). Enjoy! 

[1]: http://www.icndb.com/api/
[2]: http://www.sublimetext.com/2
[3]: http://pythonturtle.org/
[4]: http://docs.python.org/2/library/turtle.html
