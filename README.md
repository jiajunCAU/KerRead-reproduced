## Kernel Readout for Graph Neural Networks
This is the implementation of KerRead proposed in our paper.
### Requirement
* python=3.9.16
* torch=1.13.0
* numpy=1.24.4
* torch-cluster=1.6.1
* torch-geometric=2.3.1
* torch-scatter=2.1.1
* torch-sparse=0.6.17
* torch-spline-conv=1.2.2
* tqdm=4.65.0  
* scipy=1.11.1
* scikit-learn=1.3.0 
* networkx=2.8.8
### Quick Start （Reproduce Experiment）
Using GAT as the backbone, conduct graph classification task in DD, NCI1 and MUTAG dataset, please run:
```
python main.py --dataset DD --gnn gat --read_op kr --kernel gaussian
python main.py --dataset NCI1 --gnn gat --read_op kr --kernel gaussian
python main.py --dataset MUTAG --gnn gat --read_op kr --kernel gaussian
```
Using GCN as the backbone, conduct graph classification task in MUTAG dataset, please run:
```
python main.py --dataset MUTAG --gnn gcn --read_op kr --kernel gaussian
```

