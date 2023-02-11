# Metaprogramming

## Basic Building Blocks
-- statements
-- functions
classes

exec(statements, # can execute
def func(x,y,z)

positional arguments
keyword arguments
default arguments - mutable vlaues

args - tuple
kwargs - is dict of keywords args

args = (1, 2) kwargs = {}

def recv(maxSize, *, block=True): # Named arguments appearing after * can only be passed by kewords

recv(8192, block=False) # ok
recv(8192, False) #Error

You can make and return functions:

```

def make_adder(x, y):
  def add():
    return x + y
  return add
a = make_adder(2, 3)
b = make_adder(10, 20)
a()
b()

```


# Big Picture:

- Debugging code is isolated to single location
- This makes it easy to change (or to disable)
- user of a decorator doesn't worry about it
- That's really the whole idea


