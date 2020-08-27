Independent Research Project
============================

Due **5pm BST on 28th August**.

Place any code developed during this project in this directory, using git/version control as normal.

Use the `Documentation` folder for any documentation/manuals you write. You are otherwise free to develop your own file structures as appropriate to your project.

You may edit this README.md if you choose.

# Predicting the spatial variationof COVID-19 infections using GenerativeAdversarial neural Networks
## Use instruction
```
git clone https://github.com/acse-2019/irp-acse-yl7419.git
cd Code
```
## Code structure

wgan9000.h5 : the trained model based on WGAN from weight clipping through 9000 epochs
wgan9000_gp_layernormlazition.h5 : the trained model based on WGAN from gradient penalty through 9000 epochs
dis_logs :  the loss of discriminator based on WGAN from gradient penalty, use tensorboard to see
gen_logs : the loss of generator based on WGAN from gradient penalty, use tensorboard to see
wgan-gp.ipynb : the training process of  WGAN from gradient penalty
wgan-gp-prediction.ipynb : the prediction of WGAN from gradient penalty
wgan-wc.ipynb : the training and prediction of WGAN from weight clipping
data_assimilation.ipynb : data assimilation process with 5 observations
