# Heart Rate (HR) Signal Features

This repository contains code for extracting time-domain and frequency-domain features from heart rate signals, facilitating further heart rate variability (HRV) analysis. A sample ECG signal is used in the Jupyter Notebook to demonstrate the entire process, including preprocessing, peak detection, and heart rate calculation, with visualizations to enhance understanding. Finally, features are extracted from segments of the heart rate signal, providing a comprehensive workflow for HRV feature extraction.  

The affectiveness of used featues are investigated through machine learning methods in below paper, so if you find this code useful, please consider citing the paper.

[**Assessing the Effectiveness of Heart Rate Variability as A Diagnostic Tool for Brain Injuries in Infants**](https://ieeexplore.ieee.org/abstract/document/10782021)

``` bash
@INPROCEEDINGS{10782021,
  author={Rezaei, K. and Yu, K. and Mathieson, S. R. and Flynn, A. and Lightbody, G. and Boylan, G.B. and Marnane, W. P.},
  booktitle={2024 46th Annual International Conference of the IEEE Engineering in Medicine and Biology Society (EMBC)}, 
  title={Assessing the Effectiveness of Heart Rate Variability as A Diagnostic Tool for Brain Injuries in Infants}, 
  year={2024},
  volume={},
  number={},
  pages={1-4},
  keywords={Support vector machines;Pediatrics;Electric potential;Time-frequency analysis;Medical services;Forestry;Electrocardiography;Feature extraction;Electroencephalography;Heart rate variability;Electrocardiogram;Heart Rate Variability;Hypoxic Ischemic Encephalopathy grading;Seizure;Time and Frequency Domain Features;Random Forest Classifier},
  doi={10.1109/EMBC53108.2024.10782021}}
```

## Extracted Features

The following features are extracted from the heart rate signal:

1. **Mean of the NN interval** (mean NN)
2. **Standard deviation of NN-interval** (SDNN)
3. **Root mean square of successive differences** between normal heartbeats (RMSSD)
4. **Triangular index** based on the NN interval histogram (TRindex)
5. **Kurtosis**
6. **Skewness**
7. **Approximate entropy** (ApEn)
8. **Poincare plot standard deviation** along the minor axis
9. **Poincare plot standard deviation** along the major axis
10. **Ratio between SD1 and SD2** (SD2/SD1)
11. **Modified cardiac sympathetic index** (CSI_Modified)
12. **Cardiac vagal index** (CVI)
13. **Very low frequency power** (VLF)
14. **Low frequency power** (LF)
15. **High frequency power** (HF)
16. **Ratio between LF and HF** (LF/HF ratio)

## Prerequisite Libraries

To run the code, make sure to have following libraries intalled:

```bash
 pip install pyhrv
 pip install biosppy
 pip install matplotlib
 pip install numpy
 pip install scipy
 pip install nolds
 pip install spectrum
 pip install neurokit2
