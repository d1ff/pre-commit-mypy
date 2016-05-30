mypy mirror
===========

Mirror of mypy package for pre-commit

For pre-commit: see https://github.com/pre-commit/pre-commit

For mypy: see http://mypy.readthedocs.io/en/latest/index.html


### Using mypy with pre-commit

Add this to your `.pre-commit-config.yaml`:

    -   repo: git://github.com/d1ff/pre-commit-mypy
        sha: ''  # Use the sha / tag you want to point at
        hooks:
        -   id: mypy

By default it uses ```--check-untyped-defs``` option with
```--silent-imports```. You may override it with ```args``` property of the
hook in your config.
