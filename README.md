
dpsa4fl example
===============

Installation & development
------------

Currently, we only support an installation from source.

You need the following tools:
- pipx
- patchelf
- a rust toolchain
- [maturin](https://github.com/PyO3/maturin)

With pipx, we are going to install a new version of `poetry` from source:
```
$ pipx install --suffix @master 'poetry @ git+https://github.com/python-poetry/poetry'
```
We can call the resulting program using `poetry@master`.

In order to work at the same time on all the packages, your directory structure must be as follows:
```
 ./
 |- flower-with-prio
 |- dpsa4fl-example
 |- dpsa4fl
```

To build, and execute example code from rust do the following:
```
$ cd dspa4fl-example
$ poetry@master install
$ python
>>> import dpsa4fl_example.main as dm
>>> dm.call_sum(2,3)
```




