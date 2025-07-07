# paylix-python-sdk

## Introduction

Paylix public API for developers to access merchant resources

## Requirements

- python ^3.7

## Installation

Install the package through pip.

```
python3 -m pip install sellix-python-sdk
```

## Usage

```python
from paylix import Paylix

# pass <MERCHANT_NAME> only if you need to be authenticated as an additional store

client = Paylix("<YOUR_API_KEY>", "<MERCHANT_NAME>")

try:
    products = client.get_products()
except Paylix.PaylixException as e:
    print(e)

```

