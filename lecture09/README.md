### Chapter 12 - Using TKinter for Better Graphics (Cont.)

#### GUI Programming

* * *

##### Text
```
>>> from tkinter import *
>>> tk = Tk()
>>> canvas = Canvas(tk, width=500, height=500)
>>> canvas.pack()
>>> canvas.create_text(150, 100, text='Once upon a time, there lived a wolf under a bridge')
>>> canvas.create_text(150, 200, text='Once upon a time, there lived a wolf under a bridge', font=('Times', 15), fill='red')
```

* * *

##### Polygons
```
>>> from tkinter import *
>>> tk = Tk()
>>> canvas = Canvas(tk, width=500, height=500)
>>> canvas.pack()
>>> points = [0, 0, 500, 250, 0, 500]
>>> canvas.create_polygon(points, outline='green', fill='yellow', width=3)
```

* * *

##### Polygon -> triangle - move
```
import time
from tkinter import *
tk = Tk()
canvas = Canvas(tk, width=400, height=400)
canvas.pack()
canvas.create_polygon(10, 10, 10, 60, 50, 35)
for x in range(0, 60):
    canvas.move(1, 5, 5)
    tk.update()
    time.sleep(0.05)
```

* * *

##### Image
```
>>> from tkinter import *
>>> tk = Tk()
>>> canvas = Canvas(tk, width=400, height=400)
>>> canvas.pack()
>>> img = PhotoImage(file='C:\\Users\\someuser\\Documents\\Projects\\cat.gif')
>>> canvas.create_image(0, 0, anchor=NW, image=img)

>>> canvas.move(1, 5, 0)

>>> def move(e):
	if e.keysym == 'Up':
		canvas.move(1, 0, -3)
	elif e.keysym == 'Down':
		canvas.move(1, 0, 3)
	elif e.keysym == 'Left':
		canvas.move(1, -3, 0)
	else:
		canvas.move(1, 3, 0)

>>> canvas.bind_all('<KeyPress-Up>', move)
>>> canvas.bind_all('<KeyPress-Down>', move)
>>> canvas.bind_all('<KeyPress-Right>', move)
>>> canvas.bind_all('<KeyPress-Left>', move)
```

* * *

### Code Combat
- https://codecombat.com
