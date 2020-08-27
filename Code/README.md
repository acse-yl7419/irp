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
## Code structure
```
Model/WGAN_WC_one_simulation.h5 : the one-simulation trained model based on WGAN from weight clipping through 9000 epochs
Model/WGAN_GP_one_simulation.h5 : the one-simulation trained model based on WGAN from gradient penalty through 9000 epochs
Model/WGAN_GP_40_simulations.h5 : the 40-simulation trained model based on WGAN from gradient penalty through 4800 epochs
Dis_logs_one_simulation :  the loss of discriminator based on WGAN from gradient penalty for one simulation, use tensorboard to see
Gen_logs_one_simulation : the loss of generator based on WGAN from gradient penalty for one simulation, use tensorboard to see
WGAN_WC.ipynb : the training and prediction of WGAN from weight clipping for one simulation
WGAN_GP.ipynb : the training process of  WGAN from gradient penalty for one simulation
WGAN_GP_prediction.ipynb : the prediction of WGAN from gradient penalty for one simulation
WGAN_GP_40_simulations.ipynb : the training and prediction processes based on WGAN fro gradient penalty method for 40 simulations
Data_assimilation.ipynb : Data assimilation process with 5 observations based on WGAN-GP
```
