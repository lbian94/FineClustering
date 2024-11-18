The codes in this repository are an additional materials for:  
Automatic Extraction of Fine Structural Information in ARPES by Multi-Stage Clustering Algorithm  
Correspondence should be addressed to Lingzhu Bian (bianlz@ihep.ac.cn)  

# Contents in this repository
**data**: The Nano-ARPES data used in this study  
  - data: the h5 file only including the 4D spatial mapping dataset, which can be directly used in the code.
  - truth_table.h5: the truth table of the sample in the paper, used to calculate the performance metrics.

**notebook**: Codes for this manuscript in Jupyter Notebook (*.ipynb) enable you to generate all figures and performance metrics
  - Main_MSCA.ipynb: The code for the main body of this manuscript, including 4 parts. Please run the 4 parts sequentially when running the code for the first time, as this process will save some data. Afterwards, you can run each part independently (**Always run Part1 every time, as it requires loading data**).
    - Part1: Data Loading and pre-processing
    - Part2: iEDCs K-means clustering
    - Part3: Multi-Stage Clustering Algorithm (MSCA)
    - Part4: Dependence of cells on the result
  - SI-C: The code for study of iEDCs K-means clustering on the data of MoS2 (Section C in the supplementary information). **Need to run Main_MSCA.ipynb first**
  - SI-D: The code for study of two distinct features (Section D in the supplementary information). **Need to run Main_MSCA.ipynb first**
  - SI-E: The code for study of Reference-based Auto-correlation Clustering (Section E in the supplementary information)
  - SI-F: The code for study of iEDCs fuzzy-c-means clustering (Section F in the supplementary information)
  - SI-G: The code for study of Principal component analysis (Section G in the supplementary information)
# Requirements
  - h5py: https://pypi.org/project/h5py/
  - PIL: https://pypi.org/project/Pillow/
  - matplotlib: https://pypi.org/project/matplotlib/
  - scikit-learn: https://pypi.org/project/scikit-learn/
  - gap-statistic: https://pypi.org/project/gap-stat/
  - scipy: https://pypi.org/project/scipy/
