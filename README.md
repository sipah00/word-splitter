# Smart Parser: ML-Based Word Splitter

This repository implements a machine learning model that splits concatenated text into meaningful words. For example, it converts `"himynameisx"` to `"hi my name is x"`. Instead of using traditional algorithms, I implemented a **Bidirectional LSTM (BiLSTM)** model and trained it on text data to solve the problem.

## How This Problem Came Up
While exploring interesting machine learning problems, I stumbled upon the problem of converting concatenated text into properly spaced sentences, such as transforming `"hellohowareyou"` into `"hello how are you"`. The challenge required designing a **machine learning-based solution**, not a traditional algorithmic one. This inspired me to experiment with building a model from scratch, starting with a BiLSTM approach and using the [BookCorpus dataset](https://huggingface.co/datasets/bookcorpus/bookcorpus) for training.

## Example Predictions
| Input                         | Output                      |
|-------------------------------|-----------------------------|
| `mynameisshubham`                 | `hi my name is shubham`           |
| `thequickbrownfoxjumpsoverthelazydog` | `the quick brown fox jumps over the lazy dog` |
| `machinelearningisfun`        | `machine learning is fun`   |
| `iloveprogramming`            | `i love programming`        |
| `hellohowareyou`              | `hello how are you`         |

## Next Steps
This is the first iteration of the project, and the initial results are promising. Next steps include:
- Experimenting with BERT or GPT models for better contextual understanding.
- Improving edge case handling, such as for rare words or ambiguous splits.
- Extending the dataset to cover more diverse and complex scenarios.
