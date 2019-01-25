* * *

* [Presentation for Week 7](https://docs.google.com/presentation/d/1FUcFb78FCY9WI3JxZdZJAR-JmhqIJ4gZu3GnRlptivg/edit?usp=sharing)


### Review of Homework


* * *

### Let's Practice Typing
- Go to [Nitro Type](https://www.nitrotype.com)
- Practice typing for 5 minutes
- Let's measure your typing speed

* * *

### Chapter 10 - Useful Python Modules

##### turtle
```
>>> import turtle
```

##### random
```
>>> import random
>>> A = [10, 20, 30, 40, 50]
>>> random.choice(A)
50
>>> random.choice(A)
30
>>> random.choice(A)
50
>>> random.choice(A)
30
>>> random.choice(A)
40
```

##### time
```
>>> import time
>>> time.time()
1511711769.7801137
>>> time.time()
1511711773.4365573
>>> time.asctime()
'Sun Nov 26 07:56:51 2017'
>>> time.localtime()
time.struct_time(tm_year=2017, tm_mon=11, tm_mday=26, tm_hour=7, tm_min=57, tm_sec=12, tm_wday=6, tm_yday=330, tm_isdst=0)
>>> time.localtime()[0]
2017
>>>
```

##### pickle
```
>>> A = [10, 20, 30, 40, 50]
>>> import pickle
>>> pickle.dump(A, open('my_data.p', 'wb'))

# Close IDLE and re-launch IDLE
>>> A = pickle.load(open('my_data.p','rb'))
>>> A
[10, 20, 30, 40, 50]
```

* * *

### Code Combat
- https://codecombat.com
