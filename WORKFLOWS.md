# Python Workflows


### "I want to find out if certain functionality exists in Python already."
* Check out the Official Python Documentation's **Library Reference**, which lists all modules in the standard library and determine which module _could_ include your needed functionality: [[Link]](https://docs.python.org/3/library/index.html)

### "I want to find out if someone in the Python community has written certain functionality."
* **First Option:** Search for functionality by topic or keyword in the PyPi package directory: [[Link]](https://pypi.org/)
* **Second Option:** Search GitHub (or other VCS) for Python packages in your version of Python: [[Link]](https://github.com/topics/python)

### "I want to know if my code is 'good.'"
* Install & run syntax checkers, like `pylint` to analyze your code and output suggested changes: [[Link]](http://pylint.pycqa.org/en/latest/)
* Write basic unit tests to verify your code's logic, such as with `unittest` & `pytest`: [[#1]](https://docs.python.org/3.6/library/unittest.html) & [[#2]](https://docs.pytest.org/en/latest/)
* Can your code be explained simply? Does it include docstrings and/or a README file?
* Has your intended "User" tested your program? Does it behave as intended?
* Can it be installed by the intended "User" or within a simulated User-environment?

### "I want to share my code with the world! Where do I start?"
* **Fast:** Use GitHub Repositories & Gists to share projects and snippets with others on the Web.
* **Solid:** Use PyPi to structure, package, register, and distribute your Python package publicly.
* **Bad:** Share `.py` file with people via email attachment.
* **Terrible:** Take picture of code and post to Instagram.
