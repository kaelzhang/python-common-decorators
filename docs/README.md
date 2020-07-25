[![](https://travis-ci.org/kaelzhang/python-common-decorators.svg?branch=master)](https://travis-ci.org/kaelzhang/python-common-decorators)
[![](https://codecov.io/gh/kaelzhang/python-common-decorators/branch/master/graph/badge.svg)](https://codecov.io/gh/kaelzhang/python-common-decorators)
[![](https://img.shields.io/pypi/v/common-decorators.svg)](https://pypi.org/project/common-decorators/)
[![](https://img.shields.io/pypi/l/common-decorators.svg)](https://github.com/kaelzhang/python-common-decorators)

# common-decorators

Delightful Python decorators for daily use

## Install

```sh
$ pip install common-decorators
```

## Usage

```py
from common_decorators import (
  lazy
)
```

### @lazy

Defines a getter property and will assign the attribute as a normal value after the first get

```py
class Foo:
    @lazy
    def bar(self):
        return theVeryHeavyCalculation()

foo = Foo()

print(foo.bar)
```

## License

[MIT](LICENSE)
