# CMPT-GUI-starter-pack

```python
from tkinter import *

class GUI:
        def __init__(this):
            this.myWindow = Tk()
            mainloop()

gui = GUI()
```
`------------------------`
```python
from tkinter import *

class GUI:
        def __init__(this):
            this.window = Tk()

            this.label = Label(this.window, text="Hello World")
            this.label.place(x=20,y=20)
            
            mainloop()

gui = GUI()
```
`------------------------`
```python
from tkinter import *

class GUI:
        def __init__(this):
            this.window = Tk()

            # Determine the size and location of the main window
            this.window.geometry("500x300+200+100")
            
            this.label = Label(this.window, text="Hello World")
            this.label.place(x=100,y=100)
            
            mainloop()

gui = GUI()
```
`------------------------`
```python
from tkinter import *

class GUI:
        def __init__(this):
            this.window = Tk()

            # Determine the size and location of the main window
            this.window.geometry("500x300+200+100")

            # Frame A
            this.frameA = Frame(this.window, width=280, height=140, bg="yellow")
            this.frameA.place(x=10,y=10)

            # Frame B
            this.frameB = Frame(this.window, width=280, height=140, bg="green")
            this.frameB.place(x=10,y=150)
            
            this.label = Label(this.window, text="Hello World", bg="green")
            this.label.place(x=100,y=100)
            
            mainloop()

gui = GUI()
```
`------------------------`
