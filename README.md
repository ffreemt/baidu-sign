# baidu-sign
[![pytest](https://github.com/ffreemt/baidu-sign/actions/workflows/routine-tests.yml/badge.svg)](https://github.com/ffreemt/baidu-sign/actions)[![python](https://img.shields.io/static/v1?label=python+&message=3.8%2B&color=blue)](https://www.python.org/downloads/)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)[![PyPI version](https://badge.fury.io/py/baidu_sign.svg)](https://badge.fury.io/py/baidu_sign)

Sign text for baidu fanyi

## Intro
`baidu_sign` makes use of `google_sign` for text shorter than 31 characters which is about
30 times faster than `js2py_sign`. `google_sign` is a direct python implementation
while `js2py_sign` is converted from js to python using `js2py`.

## Install it
```
pip install baidu-sign
```
## Use it
```python
from baidu_sign import baidu_sign

print(baidu_sign("test"))
# "431039.159886"

print(baidu_sign("test " * 10))
# "403909.183028"
