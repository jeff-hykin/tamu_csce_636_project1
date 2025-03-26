## (Readme template below)

# What is this?

Just a tool for tamu_csce_636

# How do I use this?

`pip install tamu_csce_636_project1`


```python
from tamu_csce_636_project1 import Evaluator

evaler = Evaluator(
    first_name="Your Name",
    last_name="Your Name",
    email="your email@tamu.edu",
    print=True,
)

#                           #
### your normal code here ###
#                           #

σ = evaler.eval(
    func=lambda *args: [1],
    # your_func will be given k (int), n (int), m (int),
    # and p_list, which will be a list of P matrices, each as a numpy array
)

# use your own inputs/outputs
σ = evaler.eval(
    inputs={
        # n,k,m
        '[5,2,2]': [
            # P matrix #1
            numpy.array([
                [ 0.4759809,  0.9938236, 0.819425 ],
                [-0.8960798, -0.7442706, 0.3345122],
            ]),
            # ... (additional P matrices here)...
        ],
    },
    outputs={
        # n,k,m
        '[5,2,0]': [
            1 # correct output for first P matrix
        ],
        '[5,2,2]': [
            1.9242387 # correct output for second P matrix
        ]
    },
    func=YOUR_FUNC_HERE,
)
```
