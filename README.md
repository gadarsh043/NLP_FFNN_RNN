# Assignment 2: Neural Networks for Text Classification

This repository contains starter code for implementing and training Feed-Forward Neural Networks (FFNN) and Recurrent Neural Networks (RNN) for text classification tasks.

## 📋 Overview

The assignment requires you to complete the forward pass implementation in both `ffnn.py` and `rnn.py`. Add the corresponding lines under the `[to fill]` comments in the `forward()` method of each class.

## 🚀 Quick Start

### Prerequisites

- Python 3.8.x
- Virtual environment (already set up in this repository)

### Setup

1. **Activate the virtual environment:**

```bash
source venv/bin/activate && python --version && which python
```

2. **Deactivate when done:**

```bash
deactivate
```

## 💻 Usage

### FFNN (Feed-Forward Neural Network)

Train a feed-forward neural network with the following command:

```bash
python ffnn.py --hidden_dim 10 --epochs 1 --train_data training.json --val_data validation.json
```

**Example with default data files:**

```bash
python ffnn.py --hidden_dim 10 --epochs 1
```

### RNN (Recurrent Neural Network)

Train a recurrent neural network with the following command:

```bash
python rnn.py --hidden_dim 32 --epochs 10 --train_data training.json --val_data validation.json
```

**Example with default data files:**

```bash
python rnn.py --hidden_dim 32 --epochs 10
```

### Command Line Arguments

| Argument | Short | Required | Default | Description |
|----------|-------|----------|---------|-------------|
| `--hidden_dim` | `-hd` | Yes | - | Hidden dimension size |
| `--epochs` | `-e` | Yes | - | Number of training epochs |
| `--train_data` | - | No | `training.json` | Path to training data |
| `--val_data` | - | No | `validation.json` | Path to validation data |
| `--test_data` | - | No | `to fill` | Path to test data |
| `--do_train` | - | No | - | Flag to enable training |

## 📁 Files

- `ffnn.py` - Feed-forward neural network implementation
- `rnn.py` - Recurrent neural network implementation
- `training.json` - Training dataset
- `validation.json` - Validation dataset
- `test.json` - Test dataset
- `word_embedding.pkl` - Pre-trained word embeddings (required for RNN)

