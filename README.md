# brent-search

[![PyPIl](https://img.shields.io/pypi/l/brent-search.svg?style=flat-square)](https://pypi.python.org/pypi/brent-search/)
[![PyPIv](https://img.shields.io/pypi/v/brent-search.svg?style=flat-square)](https://pypi.python.org/pypi/brent-search/)
[![Anaconda-Server Badge](https://anaconda.org/conda-forge/ndarray_listener/badges/version.svg)](https://anaconda.org/conda-forge/ndarray_listener)
[![Documentation Status](https://readthedocs.org/projects/brent-search/badge/?style=flat-square&version=latest)](http://brent-search.readthedocs.io/en/latest/?badge=latest)

Brent's method for univariate function optimization.

## Example

```python
from brent_search import brent

def func(x, s):
  return (x - s)**2 - 0.8

r = brent(lambda x: func(x, 0), -10, 10)
print(r)
```
The output should be
```
(0.0, -0.8, 6)
```

## Install

The recommended way of installing it is via
[conda](http://conda.pydata.org/docs/index.html)
```bash
conda install -c conda-forge brent_search
```

An alternative way would be via pip
```bash
pip install brent_search
```

## Running the tests

After installation, you can test it
```
python -c "import brent_search; brent_search.test()"
```
as long as you have [pytest](http://docs.pytest.org/en/latest/).

## Authors

* **Danilo Horta** - [https://github.com/Horta](https://github.com/Horta)

## License

This project is licensed under the MIT License - see the
[LICENSE](LICENSE) file for details
