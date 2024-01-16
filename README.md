
Certainly! Let's go through another method using a more structured layout and incorporating best practices for creating Python packages. We'll use a project structure that includes separate directories for source code, tests, and documentation.

#Project Structure
```python
mypackage/
|-- mypackage/
|   |-- __init__.py
|   |-- module1.py
|   |-- module2.py
|-- README.md
|-- setup.py
```

```python
mkdir mypackage
cd mypackage

```

```python
mkdir mypackage

```

```python
touch mypackage/module1.py
touch mypackage/module2.py

```


```python
def my_function():
    print("Hello from module1")

```

```python
touch mypackage/__init__.py

```

```python
touch setup.py

```

```python
from setuptools import setup, find_packages

setup(
    name='mypackage',
    version='0.1',
    packages=find_packages(),
)

```

```python
touch README.md

```

```python
pip install setuptools wheel

```


```python
python setup.py sdist bdist_wheel
pip install .

```

```python
from mypackage import module1

module1.my_function()

```


```python
python test_script.py

```

```python
output:-
Hello from module1

```

```python

```
