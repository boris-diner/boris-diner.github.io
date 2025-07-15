+++
title = "First Post"
date = 2025-07-15
description = """
A quick test post to try out the blog and run a little Python.
"""
+++

## First Post

Welcome to the blog!  
This is just a short post to test the formatting, play with some code, and make sure everything looks good.

Here’s a tiny Python snippet to simulate a basic sine wave.

## Python Example: A Simple Sine Wave

```python
import numpy as np
import matplotlib.pyplot as plt

# Time array: 0 to 1 second, 1000 samples
t = np.linspace(0, 1, 1000)
# Sine wave: 5 Hz
y = np.sin(2 * np.pi * 5 * t)

plt.plot(t, y)
plt.title("5 Hz Sine Wave")
plt.xlabel("Time (s)")
plt.ylabel("Amplitude")
plt.grid(True)
plt.show()
```
## Julia Example: A Tiny Moving Average Filter
```julia
using DSP

# Define a simple moving average filter
h = [1, 1, 1] ./ 3  # 3-point averaging kernel

# Define an impulse signal
x = [1.0; zeros(9)]

# Compute the output via convolution
y = conv(x, h)

println("Impulse response: ", y)
```