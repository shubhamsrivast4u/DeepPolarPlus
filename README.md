# DeepPolar+: Breaking the BER-BLER Trade-off with Self-Attention and SMART (SNR-MAtched Redundancy Technique) decoding

This repository contains the implementation of 
S. Srivastava and A. Banerjee, "DeepPolar+: Breaking the BER-BLER Trade-off with Self-Attention and SMART (SNR-MAtched Redundancy Technique) decoding".

![deeppolar_snr](https://github.com/user-attachments/assets/0bb0ce3e-f491-4055-98cb-3aa741c931b5)


## Repository Structure

- `deeppolar_plus_Xepochs.ipynb`: Training notebooks for X epochs
- `deeppolar_plus_training_snr_Y_changed-300epochs.ipynb`: Training with SNR pairs (Y, Y-2)
- `SMART-CRCZ.ipynb`: DP+SMART decoder implementation with CRC length Z
- `gfchanged/`: Modified kernel training code with DeepPolar+ g and f functions
- `DeepPolar/`: Saved model weights and experimental results

## Implementation Notes

- All notebooks labeled "DeepPolar" in plots refer to DeepPolar+ models with specific training configurations
- Results for different parameter settings are organized in separate notebooks for clarity
- Training configurations explored:
  - Multiple epoch durations
  - Various SNR training pairs
  - Different CRC lengths for DP+SMART decoder

## Acknowledgement

This work builds upon the DeepPolar codebase: https://github.com/hebbarashwin/deeppolar


