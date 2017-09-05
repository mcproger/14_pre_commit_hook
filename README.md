# Quadratic Equations Solver

A small script that works through githooks and can interrupt commit changes before this happens if some of the tests are interrupted.


# Using 

For using this feature you should make few actions:
  * Copy `pre-commit` into file `.git/hooks` directory;
  * Make this script executable - ` $ chmod + x .git/hooks/pre-commit`.
  
After that, if you try to commit some changes with broken tests, the pre-commit hook will cancel it and show an error message.

```
$ git commit -m "Some changes"
  Ran 4 tests in 0.001s

  FAILED (errors=1)
  Makefile:5: ошибка выполнения рецепта для цели «test»
  make: *** [test] Ошибка 1
```


# Run tests

For running the tests in directory of project make:

```
$ python3 tests.py
```


# Project Goals

The code is written for educational purposes. Training course for web-developers - [DEVMAN.org](https://devman.org)
