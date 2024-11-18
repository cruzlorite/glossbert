# GlossBERT Wrapper Class

This Python package provides a convenient wrapper for using [GlossBERT](https://github.com/HSLCY/GlossBERT/tree/master), allowing you to easily perform word sense disambiguation (WSD) by searching WordNet through NLTK.

The source code found in this repository is an adaptation from: https://github.com/HSLCY/GlossBERT/blob/master/run_infer_demo_sent_cls_ws_with_nltk.py

## Features

- Simplifies the use of GlossBERT for WSD tasks.
- Provides integration with WordNet via NLTK.

## TODO

- [ ] Implement batch processing support in GlossBERT to enable more efficient inference for multiple words.

## Installation

Install the package using pip:

```bash
pip install glossbert
```

Alternatively, install directly from the GitHub repository:

```bash
pip install git+https://github.com/cruzlorite/glossbert.git
```

## Usage

Here is an example of how to use the GlossBERT class:

```python
from glossbert import GlossBERT

# initialize the GlossBERT instance
gloss = GlossBERT()

# define a sentence and specify the target word
sent = "I love dogs!"
start_idx, end_idx, target_word = 7, 11, "dog"

# perform word sense disambiguation
result = gloss(sent, start_idx, end_idx, target_word)

print(result)
```

## License

This project is licensed under the [MIT License](https://opensource.org/license/mit), consistent with the original [GlossBERT project](https://github.com/HSLCY/GlossBERT/tree/master).

## Acknowledgements

Special thanks to the authors of the original [GlossBERT](https://github.com/HSLCY/GlossBERT/tree/master) for their foundational work.