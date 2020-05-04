# Call function by string value

If you need to call a function based on the value in a string object
you can use the [`getattr`](https://docs.python.org/3/library/functions.html#getattr) method.

**If the function is in an object**

```python
class A:
  def foo(self):
    print('bar')

a = A()
x = 'foo'
func = getattr(a, x)
func()
# bar
```

**If the function is not in an object**
```python
import sys

def foo:
  print('bar')

x = 'foo'
current_module = sys.modules[__name__]
func = getattr(current_module, x)
func()
# bar
```
