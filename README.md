# iterative Structural Inference of Directed Graphs (iSIDG)

This repository is the official implementation of iterative Structural Inference of Directed Graphs (iSIDG).

## Requirements

To install requirements:

* [PyTorch](https://pytorch.org/get-started/locally/)
* [scikit-learn](https://scikit-learn.org/stable/getting_started.html) 
* (Optional) CUDA GPU support. If you don't have it, you can run the training script with "--no-cuda" arg.

## Data Generation

For instance to create the springs dataset:
```
python data/generate_physics_dataset.py
```
To create the charged particles dataset:
```
python data/generate_physics_dataset.py --simulation 'charged'
```
To create the Kuramoto dataset:
```
python data/generate_kuramoto_dataset.py
```
For synthetic networks and NetSim datasets, we sampled them already and stored in "data/netsims" and "data/Synthetic-H/sampled_data". 



## Example Run

For instance to start a training session:
```
python train.py
```
For different datasets, use corresponding args to run the experiments.

