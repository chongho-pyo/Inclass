# Decision Analytics

## Contents
- Linear Optimization
  - Modeling business problems as LP
  - Solving LP problems in Gurobi
  - Sensitivity analysis
  - Solving LP problems in Gurobi and sensitivity analysis
  - Duality: An economic interpretation of LP
  - LP and uncertainty

- Discrete Optimization
  - Modeling business problems as discrete optimization
  - Solving discrete optimization problems in Python
  - Travelling salesman problem (TSP)
  - Graphical solutions to MIP
  - Branch and bound method
  - Application of discrete optimization in machine learning (Clustering)
        
- Non‐Linear Optimization
  - Modeling business problems as NLP
  - Graphical solution to NLP
  - Sensitivity analysis
  - Gradient descent method for unconstrained optimization
  - Karush‐Kuhn‐Tucket conditions for constrained nonlinear optimization
  - Application of NLP in machine learning (Support Vector Machines)
  
## Group Project
### Problem Description
- The goal is to allocate optimal inventory for each smartphone device according
to 5 different warehouses’ predicted demand.
- This will result in maximizing profit, which is measured by subtracting fixed and variable costs from the revenue. 
- The variable costs include shipping cost and overstocking fee whereas the fixed costs consist of transfer
cost and maintenance cost.

### Parameters
<img width="724" alt="image" src="https://user-images.githubusercontent.com/75922678/223590346-2623be67-ae00-4241-bc3b-ca90ab8637ba.png">

### Decision Variables
<img width="505" alt="image" src="https://user-images.githubusercontent.com/75922678/223590479-c906740e-0fed-499d-9545-f8823456e636.png">

### Model Formulation

#### Objective Function
<img width="520" alt="image" src="https://user-images.githubusercontent.com/75922678/223590587-4ff704c8-9b0f-4f2d-b6c8-fd7ed938bf5b.png">

#### Objective Function with Parameters
<img width="499" alt="image" src="https://user-images.githubusercontent.com/75922678/223590648-f17a4aed-8c33-445c-bb61-2c9570801016.png">

### Constraints
<img width="414" alt="image" src="https://user-images.githubusercontent.com/75922678/223590871-23c1da2a-5f81-4fe3-aa7e-642b5a4f8ce7.png">

<img width="553" alt="image" src="https://user-images.githubusercontent.com/75922678/223590922-43ef4fff-e07a-45d1-9b3d-8e5b38d5aad4.png">

### Elaboration
#### Overstocking
<img width="539" alt="image" src="https://user-images.githubusercontent.com/75922678/223591008-a19e2549-4347-4350-9049-8985706828dc.png">


### Result
- Compare to the previous inventory plan without our optimization solution, we could demonstrate that the overall net profit increased by about 59070 in US dollars due to the increase in the total number of products and reduce in the cost of overstocking.
- The key feature here is the overstocking issue has been reduced but the actual total number of products sold are increased in our model. This indicates that we made better allocations to meet the demand as much as possible and minimize the overstocking of each warehouse in the meantime.

<img width="666" alt="image" src="https://user-images.githubusercontent.com/75922678/223591339-ac739587-0222-496e-a960-5af3b93ec0c1.png">

