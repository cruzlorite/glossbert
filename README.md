# GlossBERT Python Wrapper Class

This python package offers a wrapper class to use [GlossBERT](https://github.com/HSLCY/GlossBERT/tree/master) easily.


# Instalation

Using `pip`:

```bash
pip install glossbert
```

From github:

```bash
pip install glossbert
```

# Usage

Import the `GlossBERT` class from the `glossbert` package:

```python
>>> from glossbert import GlossBERT
>>>
>>> gloss = GlossBERT()
>>> sent = "I love dogs!"
>>> result = gloss(sent, 7, 11, "dogs")
>>> print(result)
>>>
```

# License

This project is licensed under the MIT license, like the original [GlossBERT](https://github.com/HSLCY/GlossBERT/tree/master).
