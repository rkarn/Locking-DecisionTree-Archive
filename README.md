# Locking-DT-RF

The step-by-step annotated source code is available in the Jupyter notebook file. It uses MNIST dataset. 

The locking simulated in software is available in "MNIST Decision Tree Random Key locking.ipynb". The logic to generate the Verilog HDL file is also given this jupyter notebook.

Once the HDL state machine is generated, then the RTL FSM is copied from the respective ".v" file and paste in the Quartus project. It is follwed by the synthesis, bitstream generation, and, finally, demonstration on the FPGA board. 

The quartus project is given in folders "XOR_all_nodes", "XNOR_all_nodes", "XOR_XNOR_all_nodes", and "XOR_XNOR_Some_nodes". After the "sof" (bitstream) file is generated, it is loaded into the FPGA. The demo of inferencing for the  "XOR_XNOR_Some_nodes" case is shown in video "demo - XOR_XNOR_Some_nodes". The jupyter notebook file to show the inferencing demo is "LockedDecisionTreeInferencing.ipynb".

Decision Tree Architecture:
![alt text](https://github.com/rkarn/Locking-DT-RF/blob/main/decision_tree_diagram-1.png)


Locked Decision Treee Architecture:
![alt text](https://github.com/rkarn/Locking-DT-RF/blob/main/Locked_decision_tree.png)


In future, the locking of random forest will be added. 
