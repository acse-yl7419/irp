Independent Research Project
============================

Due **5pm BST on 28th August**.

Place any code developed during this project in this directory, using git/version control as normal.

Use the `Documentation` folder for any documentation/manuals you write. You are otherwise free to develop your own file structures as appropriate to your project.

You may edit this README.md if you choose.

# Predicting the spatial variationof COVID-19 infections using Generative Adversarial neural Networks
## Use instruction
```
git clone https://github.com/acse-2019/irp-acse-yl7419.git
cd Code
```
## File description

Model/one_simulation_wgan_wc.h5 : the one-simulation trained model based on WGAN from weight clipping through 9000 epochs
Model/one_simulation_wgab_gp.h5 : the one-simulation trained model based on WGAN from gradient penalty through 9000 epochs
Model/40_simulations_wgan_gp.h5 : the 40-simulation trained model based on WGAN from gradient penalty through 4800 epochs
one_simulation_dis_logs :  the loss of discriminator based on WGAN from gradient penalty for one simulation, use tensorboard to see
one_simulation_gen_logs : the loss of generator based on WGAN from gradient penalty for one simulation, use tensorboard to see
one_simulation_wgan_wc.ipynb : the training and prediction of WGAN from weight clipping for one simulation
one_simulation_wgan_gp.ipynb : the training process of  WGAN from gradient penalty for one simulation
one_simulation_wgan_gp_prediction.ipynb : the prediction of WGAN from gradient penalty for one simulation
40_simulations_wgan_gp_training1.ipynb : the training 1 based on WGAN from gradient penalty method for 40 simulations through the first 3100 epochs
40_simulations_wgan_gp_training2.ipynb : the training 2 based on WGAN from gradient penalty method for 40 simulations through the next 1900 epochs
40_simulations_wgan_gp_prediction.ipynb : the prediction process based on WGAN from gradient penalty method for 40 simulations
da_1_obs.ipynb : data assimilation process with 1 observations based on WGAN-GP
da_5_obs.ipynb : data assimilation process with 5 observations based on WGAN-GP
da_5_obs_fix_R0s.ipynb : data assimilation process with 5 observations based on WGAN-GP when fixing R0s
