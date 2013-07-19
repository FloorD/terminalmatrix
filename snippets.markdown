# Snippets


http://www.siafoo.net/article/52


```
string = 'Hi there' # True example
2# string = 'Good bye' # False example
3if 'Hi' in string:
4    print 'Success!'
```





http://pythonturtle.org/




http://stackoverflow.com/questions/101268/hidden-features-of-python

Chaining comparison operators

<pre>
>> x = 5
>>> 1 < x < 10
True
>>> 10 < x < 20
False
>>> x < 10 < x*10 < 100
True
>>> 10 > x <= 9
True
>>> 5 == x > 4
True

</pre>



http://stackoverflow.com/a/1024693
rot13 valid source encoding

#!/usr/bin/env python
# -*- coding: rot13 -*-

cevag "Uryyb fgnpxbiresybj!".rapbqr("rot13")






Conditional Assignment

x = 3 if (y == 1) else 2

Wrapping Functions

<pre>
def my_decorator(func):
    def decorated():
        print("before hallo")
        func()
        print("after hallo")
    return decorated

@my_decorator
def hallo():
    print("hallo")

hallo()
</pre>

Generating Lists from other Lists

<pre>
a = [1,2,3,4,5,6]
b = [i for i in a if i % 2 == 0] # [2, 4, 6]
</pre>

Opening Files without handling closing and such

<pre>
with open("some_file.txt", "r") as f:
   print f.read()
</pre>

Easter Eggs:
>>>import __hello__

>>> from __future__ import braces
  File "<stdin>", line 1
SyntaxError: not a chance

>>> import this
The Zen of Python, by Tim Peters

Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!


http://www.wefearchange.org/2010/06/import-this-and-zen-of-python.html


 >>> import this

>>> love = this
>>> this is love
True
>>> love is True
False
>>> love is False
False
>>> love is not True or False
True
>>> love is not True or False; love is love
True
True



import antigravity
