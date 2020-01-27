# Python Unit test template creator

A very simple utility to create a unittest template from a python file

## Installation

Just download the ```pytest``` file, add it to your somewhere in your PATH, and make it executable with

```zsh
chmod +x pytest
```

## Usage

Assuming you're in your module's directory:

```zsh
pytest [your_module].py
```

A new file will be created with the following template

```python
import unittest
import [your_module]

class Test[YourModule](unittest.TestCase):

    def test_foo(self):
        pass

    def test_bar(self):
        pass
      
if __name__ == "__main__":
    unittest.main()

```

## Notes

- Only tested for python3
- Indentation style is 4 spaces. If someone requests it, I can set up flags to specify tab preference and size, but you can modify the script to make it however you want by changing the variables `TAB_PREF` and `TAB_SIZE`.