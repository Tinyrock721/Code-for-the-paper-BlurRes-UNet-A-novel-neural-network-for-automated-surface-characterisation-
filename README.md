# BlurRes-UNet: A Novel Neural Network for Automated Surface Characterisation

This repository contains the source code for the paper:

**Cui, W., Lou, S., Zeng, W., Kadirkamanathan, V., Qin, Y., Scott, P. J., & Jiang, X. (2025). BlurRes-UNet: A novel neural network for automated surface characterisation in metrology. Computers in Industry, 165, 104228.**  
DOI: [https://doi.org/10.1016/j.compind.2025.104228](https://doi.org/10.1016/j.compind.2025.104228)

## Citation
If you use this code, please cite our paper:

```bibtex
@article{Cui2025BlurResUNet,
  title={BlurRes-UNet: A novel neural network for automated surface characterisation in metrology},
  author={Cui, Weixin and Lou, S. and Zeng, W. and Kadirkamanathan, V. and Qin, Y. and Scott, P. J. and Jiang, X.},
  journal={Computers in Industry},
  volume={165},
  pages={104228},
  year={2025},
  publisher={Elsevier}
}

## Contents
- `FR_BlurRes-UNet_v2.ipynb`: Jupyter Notebook with the source code.
- `FR_blurres-unet_v2.py`: Python file with the source code.

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/BlurRes-UNet-Surface-Characterisation.git

2. Data and Label
   Upload the dataset and labels required for the regression task into the appropriate directory. Update the file paths in the code to reflect the location of the uploaded files.
   # Read data
  dir1 = '/content/sample_data/Data'
  dir2 = '/content/sample_data/Label'

  data_files = sorted([os.path.join(dir1, f) for f in os.listdir(dir1) if f.endswith('.xlsx')])

  label_files = sorted([os.path.join(dir2, f) for f in os.listdir(dir2) if f.endswith('.xlsx')])
