# baidu-sign

Sign text for baidu fanyi

## Intro
`baidu-sign` makes use of `google_sign` for text shorter than 31 characters which is about
30 times faster than `js2py_sign`. `google_sign` is a direct python implementation
while `js2py_sign` is converted from js to python using `js2py`.

## Install it
```
pip install baidu-sign
```
## Use it
```python
from baidu_sign import baidu_sign

print(baidu_sign("test")
# "431039.159886"

print(baidu_sign("test " * 10))
# 403909.183028
