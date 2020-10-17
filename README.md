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
```python
from tkinter import *

class GUI:
        def __init__(this):
            this.window = Tk()

            # Determine the size and location of the main window
            this.window.geometry("500x300+200+100")

            # Windows title
            this.window.title("Douglas College")

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
```python
from tkinter import *

class GUI:
        def __init__(this):
            this.window = Tk()

            # Determine the size and location of the main window
            this.window.geometry("500x300+200+100")

            # Windows title
            this.window.title("Douglas College")

            # Frame A
            this.frameA = Frame(this.window, width=280, height=140, bg="yellow")
            this.frameA.place(x=10,y=10)
            
            this.label = Label(this.window, text="Hello World", bg="green", fg="green", font=("Arial", 16))
            this.label.place(x=20,y=20)

            this.button = Button(this.frameA, text="Click", bg="red", fg="blue", font=("Arial", 16))
            this.button.place(x=20, y=50)
            
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

            # Windows title
            this.window.title("Douglas College")

            # Frame A
            this.frameA = Frame(this.window, width=280, height=140, bg="yellow")
            this.frameA.place(x=10,y=10)
            
            this.label = Label(this.window, text="Hello World", bg="green", fg="green", font=("Arial", 16))
            this.label.place(x=20,y=20)

            this.button = Button(this.frameA, text="Click", bg="red", fg="blue", font=("Arial", 16), command=this.functionA)
            this.button.place(x=20, y=50)
            
            mainloop()

        def functionA (this):
                print("Clicked...")
                
gui = GUI()
```
`------------------------`
```python
from tkinter import *
import tkinter.messagebox

class GUI:
        def __init__(this):
            this.window = Tk()

            # Determine the size and location of the main window
            this.window.geometry("500x300+200+100")

            # Windows title
            this.window.title("Douglas College")

            # Frame A
            this.frameA = Frame(this.window, width=280, height=140, bg="yellow")
            this.frameA.place(x=10,y=10)
            
            this.label = Label(this.window, text="Hello World", bg="green", fg="green", font=("Arial", 16))
            this.label.place(x=20,y=20)

            this.button = Button(this.frameA, text="Click", font=("Arial", 16), command=this.functionA)
            this.button.place(x=20, y=50)

            this.exitButton = Button(this.frameA, text="Exit", font=("Arial", 16), command=this.window.destroy)
            this.exitButton.place(x=20, y=100)
            
            mainloop()

        def functionA (this):
                tkinter.messagebox.showinfo("Response", "Clicked...")
                
gui = GUI()
```
`------------------------`
GUI - Capital Cities
```python
from tkinter import *
import tkinter.messagebox

class GUI:
        def __init__(this):
            this.window = Tk()

            # Determine the size and location of the main window
            this.window.geometry("600x400+200+100")

            # Windows title
            this.window.title("Douglas College")

            # Frame A
            this.frameA = Frame(this.window, width=280, height=300, bg="green")
            this.frameA.place(x=10,y=10)
            
            this.label = Label(this.window, text="Hello World", bg="red", fg="white", font=("Capital Cities", 16))
            this.label.place(x=20,y=20)

            this.countryAButton = Button(this.frameA, text="Canada", font=("Arial", 16), command=this.canadaCapitalCity)
            this.countryAButton.place(x=10, y=50)

            this.countryBButton = Button(this.frameA, text="United State of America", font=("Arial", 16), command=this.usCapitalCity)
            this.countryBButton.place(x=10, y=100)

            this.countryCButton = Button(this.frameA, text="England", font=("Arial", 16), command=this.englandCapitalCity)
            this.countryCButton.place(x=10, y=150)

            this.exitButton = Button(this.frameA, text="Exit", font=("Arial", 16), command=this.window.destroy)
            this.exitButton.place(x=10, y=200)
            
            mainloop()

        def canadaCapitalCity (this):
                tkinter.messagebox.showinfo("Response", "Ottawa")

        def usCapitalCity (this):
                tkinter.messagebox.showinfo("Response", "Washinton, D.C.")

        def englandCapitalCity (this):
                tkinter.messagebox.showinfo("Response", "London")
                
gui = GUI()
```
`------------------------`
```python
from tkinter import *
import tkinter.messagebox

class GUI:
        def __init__(this):
            this.window = Tk()

            # Determine the size and location of the main window
            this.window.geometry("600x400+200+100")

            # Windows title
            this.window.title("Douglas College")

            # Frame A
            this.frameA = Frame(this.window, width=280, height=300, bg="green")
            this.frameA.place(x=10,y=10)
            
            this.label = Label(this.window, text="Hello World", bg="red", fg="white", font=("Capital Cities", 16))
            this.label.place(x=20,y=20)

            this.entry = Entry(this.frameA, width=20, font=16)
            this.entry.place(x=10, y= 100)

            this.clickButton = Button(this.frameA, text="Click", font=("Arial", 16), command=this.entryInput)
            this.clickButton.place(x=10, y=150)
            
            this.exitButton = Button(this.frameA, text="Exit", font=("Arial", 16), command=this.window.destroy)
            this.exitButton.place(x=10, y=200)
            
            mainloop()

        def entryInput (this):
                text = this.entry.get()
                tkinter.messagebox.showinfo("Response", "You have entered " + text)
                
gui = GUI()
```
`------------------------`
```python
from tkinter import *
import tkinter.messagebox

class GUI:
        def __init__(this):
            this.window = Tk()

            # Determine the size and location of the main window
            this.window.geometry("600x400+200+100")

            # Windows title
            this.window.title("Douglas College")

            # Frame A
            this.frameA = Frame(this.window, width=280, height=300, bg="green")
            this.frameA.place(x=10,y=10)
            
            this.label = Label(this.window, text="Hello World", bg="red", fg="white", font=("Capital Cities", 16))
            this.label.place(x=20,y=20)

            this.entry = Entry(this.frameA, width=20, font=16)
            this.entry.place(x=10, y= 100)

            this.enteredText = StringVar()
            this.enteredLabel = Label(this.frameA, textvariable=this.enteredText, font=16)
            this.enteredLabel.place(x=80, y= 150)

            this.clickButton = Button(this.frameA, text="Click", font=("Arial", 16), command=this.entryInput)
            this.clickButton.place(x=10, y=150)
            
            this.exitButton = Button(this.frameA, text="Exit", font=("Arial", 16), command=this.window.destroy)
            this.exitButton.place(x=10, y=200)
            
            mainloop()

        def entryInput (this):
                text = this.entry.get()
                this.enteredText.set(text)
                tkinter.messagebox.showinfo("Response", "You have entered " + text)
                
gui = GUI()
```
