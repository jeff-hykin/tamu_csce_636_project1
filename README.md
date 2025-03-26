## (Readme template below)

# What is this?

Just a tool for tamu_csce_636

# How do I use this?

`pip install tamu_csce_636_project1`


```python
from tamu_csce_636_project1 import Evaluator

evaler = Evaluator(
    print=True,
    input_output_pairs=[
        # n, k, m, p
        ((5, 2, 0, p), 1),
        ((5, 2, 2, p), 1.9242387),
    ]
)

losses = evaler.eval(
    # p will be a numpy matrix
    # your_func_or_whatever() needs to return the m-height value
    lambda n,k,m,p: your_func_or_whatever(n,k,m,p)
)
# losses = {
#     # n, k, m
#     (5, 2, 0): 0.0,
#     (5, 2, 2): 0.8916794023379957,
# }
```
