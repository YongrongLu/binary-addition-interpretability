# Binary Addition: A Look Inside a Small Neural Network

AIPI 590 — Week 7: Mechanistic Interpretability Shark Tank.

[Open the notebook](week7_binary_addition.ipynb) · [Run in Colab](https://colab.research.google.com/github/YongrongLu/binary-addition-interpretability/blob/main/week7_binary_addition.ipynb)

I trained a small MLP to add two 2-bit numbers and investigated whether a hidden neuron responds to a carry from the lowest bit.

In the main model (seed 0), removing neuron 15 reduced correct carry answers from 4/4 to 1/4. All 12 no-carry answers stayed correct. The notebook includes activation plots, ablation results, and comparisons with other training seeds, including a run that learned only 14/16 sums.

All 16 input pairs were used for training. These results describe the model on this small task, not generalization to unseen inputs.

## Run

Open the notebook in Colab and run the cells from top to bottom. The saved notebook already includes the outputs. For a local Jupyter environment, install the dependencies with `pip install -r requirements.txt`.

Adapted from the course [starter notebook](https://github.com/AIPI-590-XAI/Duke-AI-XAI/blob/main/assignments/mechanistic_interp_starter.ipynb).
