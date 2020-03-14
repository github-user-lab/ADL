## Problem Statement
The performance of policy gradient methods is sensitive to hyperparameter settings that must be tuned for any new application. Widely used grid search methods for tuning hyperparameters are sample inefficient and computationally expensive. This paper provides a fast, efficient way to optimize hyperparameters for policy gradients methods.

## Input & Output
* Input: a policy gradients algorithm, an environment
* Output: the policy gradients algorithm will be run on that environment with optimized hyperparameters

## Requirements:
* Python3
* Tensorflow
* OpenAI Baselines
* MuJoCo

## Deliverables
*	Code to reproduce the results of the paper for A2C
*	Code to reproduce the results of the paper for TNPG
*	Code to plot the results for A2C
*	Code to plot the results for TNPG
*	Code to build and run the docker

## Run the Code
1. Add the MuJoCo key to the folder
2. Build the docker using build.sh
3. Run the docker using run.sh
4. (Optional) Change the parameters of the algorithms in the experiment_params.yaml file
5.1. To test the algorithm on A2C, run run_all_a2c_experiments.sh. Specify the desired environment in the argument. The shortened names of the environments can be found at experiment_params.yaml. For instance, to reproduce the results on the “Ant-v2” environment, run run_all_a2c_experiments.sh with “ant” as the argument.
5.2. Similarly, to test the algorithm on TNPG, run run_all_tnpg_experiments.sh. Specify the desired environment in the argument.
6. Plot the results using plots_a2c.py or plot_tnpg_and_hypers.py.

## References
[Paul, Supratik, Vitaly Kurin, and Shimon Whiteson. "Fast Efficient Hyperparameter Tuning for Policy Gradient Methods." Advances in Neural Information Processing Systems. 2019.](https://arxiv.org/pdf/1902.06583.pdf)
