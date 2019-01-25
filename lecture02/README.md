* * *


### Chapter 12 - Using TKinter for Better Graphics

#### GUI Programming

##### Tkinter
```
>>> from tkinter import *
>>> tk = Tk()
>>> btn = Button(tk, text='click here')
>>> btn.pack()
```

* * *

##### Button
```
>>> from tkinter import *
>>> tk = Tk()
>>> def hello():
	print('Hello!')
>>> btn = Button(tk, text='Click here', command=hello)
>>> btn.pack()
```

* * *

##### Button + Messagebox
```
>>> from tkinter import *
>>> from tkinter import messagebox
>>> tk = Tk()
>>> def about():
	messagebox.showinfo('About', 'GUI v1.0')


>>> btn = Button(tk, text='About', command=about)
>>> btn.pack()
```

* * *

##### Canvas
```
>>> from tkinter import *
>>> tk = Tk()
>>> canvas = Canvas(tk, width=500, height=500)
>>> canvas.pack()
>>> canvas.create_line(0, 0, 500, 500)
```

* * *

##### Line, Rectangle, Oval
```
>>> from tkinter import *
>>> tk = Tk()
>>> canvas = Canvas(tk, width=500, height=500)
>>> canvas.pack()
>>> canvas.create_line(0, 100, 200, 0, fill='red', dash=(4, 4))
>>> canvas.create_rectangle(50, 25, 150, 75, fill='blue')
>>> canvas.create_oval(250, 250, 300, 300)
```

* * *

##### Interactive drawing
```
>>> from tkinter import *
>>> tk = Tk()
>>> canvas = Canvas(tk, width=500, height=500)
>>> canvas.pack()
>>> def paint(e):
	canvas.create_oval(e.x - 1, e.y - 1, e.x + 1, e.y + 1, fill='green')
>>> canvas.bind('<B1-Motion>', paint)
>>> def clear(e):
	canvas.delete('all')
>>> canvas.bind('<Button-3>', clear) # Right-click
```

* * *

### Code Combat
- https://codecombat.com
