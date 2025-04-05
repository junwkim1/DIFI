# DIFI
Code for "Semi-Supervised Data-Integrated Feature Importance Enhances Performance and Interpretability of Biological Classification Tasks"

What's in this repository:

  - Code for training binary classification using gradient-based sparse attention transfer
  - Jupyter notebook for cancer classification using gradient-based method of semi-supervised data-integrated feature importance (DIFI) and feature map visualization
  - Code for training enzyme classification using activation-based method of DIFI 
  - Jupyter notebook for enzyme classification feature map visualization

Note that the code uses TensorFlow for attention transfer and cancer classification experiments and PyTorch for enzyme classification experiments. 

# Requirements
Install Python packages:
pip install -r requirements.txt

# Experiments
To train and view results for sparse attention transfer for binary classification do:
python binary_classification_AT.py

To train and view results for cancer classification use cancer_classification.ipynb

To train enzyme classification using activation-based method of DIFI do:
python enzyme_nonenzyme_classification.py --non_num 60 --alpha 3

To reproduce the figures from enzyme classification use enzyme_eval.ipynb with the following trained models:
high_attention_NONNUM_60_ALPHA_3.pth for RN3
high_attention_ALPHA0.pth for RN
high_attention_NONNUM_60_random_ALPHA_3.pth for Ran3
