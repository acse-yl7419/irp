
# Predicting the spatial variationof COVID-19 infections using Generative Adversarial neural Networks
This project takes the output of a compartmental model of a simplified test case for Coronavirus disease 2019 (COVID-19) and trains Wasserstein Generative Adversarial Network (WGAN) to be able to predict spatial variations for different reproductive numbers. This project also performs data assimilation to obtain the infection state corresponding to observations. It has been demonstrated that WGAN-Gradient penalty has a good performance in COVID-19 prediction and assimilation.
## Use instruction
```
git clone https://github.com/acse-2019/irp-acse-yl7419.git
cd Code
```
## File description
- model/one_simulation_wgan_wc.h5 : the one-simulation trained model of WGAN based on weight clipping method through 9000 epochs
- model/one_simulation_wgab_gp.h5 : the one-simulation trained model based on WGAN-GP through 9000 epochs
- model/40_simulations_wgan_gp.h5 : the 40-simulation trained model based on WGAN-GP through 4800 epochs
- raw_data/one_simulation/group-output-time_mod.csv : raw data for one-simulation training and prediction
- raw_data/40_simulations/lots_run_small.zip : raw data for 40-simulation training, prediction and assimilation 
- one_simulation_dis_logs :  the loss of discriminator based on WGAN-GP for one simulation, use tensorboard to see
- one_simulation_gen_logs : the loss of generator based on WGAN-GP for one simulation, use tensorboard to see
- one_simulation_wgan_wc.ipynb : the training and prediction of WGAN based on weight clipping method for one simulation
- one_simulation_wgan_gp.ipynb : the training process of  WGAN-GP for one simulation
- one_simulation_wgan_gp_prediction.ipynb : the prediction process of WGAN-GP for one simulation
- 40_simulations_wgan_gp_training1.ipynb : the training_1 process based on WGAN-GP for 40 simulations through the first 3100 epochs
- 40_simulations_wgan_gp_training2.ipynb : the training_2 process based on WGAN-GP for 40 simulations through the next 1900 epochs
- 40_simulations_wgan_gp_prediction.ipynb : the prediction process based on WGAN-GP method for 40 simulations
- da_1_obs.ipynb : data assimilation process with 1 observations based on WGAN-GP
- da_5_obs.ipynb : data assimilation process with 5 observations based on WGAN-GP
- da_5_obs_fix_R0s.ipynb : data assimilation process with 5 observations based on WGAN-GP when fixing R0s

## Packages
This project is developed using Python 3. The developing platforms are Jupyter Notebook and Kaggle Notebook which provides access to NVIDIA K80 GPUs in kernels. The following packages are used:
- TensorFlow v2.3.0
- Numpy 1.16.4
- Scikit-Learn 0.21.3
- Matplotlib 3.1.0
