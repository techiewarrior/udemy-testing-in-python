# Notes
---


**Collect all tests in directory and subdirectories**</br>
`pytest --collect-only`


**Run all tests (call from ~/testing)**</br>
`pytest`


**... with increased verbosity**</br>
`pytest -v`


**... add coverage tests**</br>
`pytest --cov=project`


**... add PEP8 compliance testing**</br>
`pytest --pep8`


**Produce HTML testing report [(Project documentation)](https://pypi.org/project/pytest-html/)**</br>
`pytest --html=project/tests/report.html --self-contained-html`


**Clean, Lint, and Audit code**</br>
In order to clean your code and check for advanced errors, run black then lint. Black will automatically format your python code to make it more readable. Lint will check for advanced errors. The --disable=R,C arguments reduce verbosity to just warnings and errors.

```
black project/hello.py
pylint --disable=R,C project/hello.py
pytest --pep8 --disable-warnings project/hello.py
```

