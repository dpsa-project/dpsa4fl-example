
installation
------------

Currently, we only support an installation from source.

You need the following tools:
- [maturin](https://github.com/PyO3/maturin)
- pipx

With pipx, we are going to install a new version of `poetry` from source:

```
    pipx install --suffix @master 'poetry @ git+https://github.com/python-poetry/poetry'
```

We can call the resulting program using `poetry@master`.

