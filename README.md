# spinglog.py

> Spinner Logger for Python

## Installation

Just `pip install spinlog` and you can use it.

## Usage

Here is a basic usage of spinlog

```python
from spinlog import LogProgress
from time import sleep

print("About to launch Spinner")
with LogProgress("I'm spinning around") as s:
    sleep(2)
    s.info("Here is an info message") # you can use warn, error, or debug
    sleep(2)
    s.log("It's so funny", symbol="😆".encode("utf-8"))
    sleep(2)
print("Spinning Over")
```

Spinlog is build on top of [halo](https://github.com/manrajgrover/halo) providing a different API
to interact with the spinner.
