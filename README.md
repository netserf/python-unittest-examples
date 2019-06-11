# python_unittest_examples v.0.1.1

## What?
A project for collecting various python unit testing tips and tricks.

The first module will be based on notes compiled from Python Testing with pytest
written by Brian Okken. Depending on how this goes there may be more modules to
come.

## Why?
I need more practice with unit testing. It seemed like a good idea at the time.

### Pytest Usage
1. Simple passing test
`$ pytest -v python_unittest_examples/ch1/test_one.py`

2. Simple failing test
`$ pytest -v python_unittest_examples/ch1/test_two.py`

3. Tests on Task namedtuple
`$ pytest -v python_unittest_examples/ch1/test_three.py`

4. More tests on Task namedtuple
`$ pytest -v python_unittest_examples/ch1/test_four.py`

5. Run a single test
`$ pytest -v python_unittest_examples/ch1/test_four.py::test_asdict`

6. Collect tests, but don't run them
`$ pytest --collect-only`

7. Run tests matching an expression
`$ pytest -v -k "asdict or defaults"`

8. Exit after first error
`$ pytest -x`

9. Exit after x failures
`$ pytest --maxfail=2`

10. Allow `print()` statements to stdout
`$ pytest -s`

11. Run the last failed test
`$ pytest --lf`

12. Show local variables for failing tests
`$ pytest -l`

13. Show the slowest N number of tests
`$ pytest --duration=N`

### Installation
```
$ pip3 install -U virtualenv
$ python3 -m virtualenv venv
$ source venv/bin/activate
$ pip install pytest
$ git clone git@github.com:netserf/python-unittest-examples.git
```
... Follow tests notes above

### Testing
```
$ python setup.py test
```

## Requirements
- pytest

## Future Improvements
- TBD

## Licence
MIT

## Authors
`python_unittest_examples` was written by `Greg Horie <networkserf@gmail.com>`

