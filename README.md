# DeepPolar+: Breaking the BER-BLER Trade-off with Self-Attention and SMART (SNR-MAtched Redundancy Technique) decoding

This repository contains the implementation of 
S. Srivastava and A. Banerjee, "DeepPolar+: Breaking the BER-BLER Trade-off with Self-Attention and SMART (SNR-MAtched Redundancy Technique) decoding".


## BER and BLER comparison with DeepPolar, Polar codes with SC decoding, RM code with Dumer Decoder, KO codes and [DKO](https://ieeexplore.ieee.org/document/10619329) codes
![deeppolar_snr](https://github.com/user-attachments/assets/0bb0ce3e-f491-4055-98cb-3aa741c931b5)


## Repository Structure

- `deeppolar_plus_Xepochs.ipynb`: Training notebooks for X epochs
- `deeppolar_plus_training_snr_Y_changed-300epochs.ipynb`: Training with SNR pairs (Y, Y-2)
- `SMART-CRCZ.ipynb`: DP+SMART decoder implementation with CRC length Z
- `gfchanged/`: Modified kernel training code with DeepPolar+ g and f functions. This is build upon [DeepPolar](https://github.com/hebbarashwin/deeppolar) codes with modified g and f function.
- `DeepPolar/`: Saved model weights and experimental results
- 'Polar_Results/curriculum/final_kernels' contains pretrained kernels with modified g and f function.

## Implementation Notes


- Results for different parameter settings are organized in separate notebooks for clarity
- Training configurations explored:
  - Multiple epoch durations
  - Various SNR training pairs
  - Different CRC lengths for DP+SMART decoder
- All notebooks labelled "DeepPolar" in plots refer to DeepPolar+ models with specific training configurations. Please ignore the labels on the plots of Jupyter Notebook files. The labels marked 'DeepPolar' are actually the results of 'DeepPolar+' models with that configuration.

## Acknowledgement

This work builds upon the DeepPolar codebase: https://github.com/hebbarashwin/deeppolar


