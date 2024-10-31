# Infant Sentiment Analysis with Pre-trained Vision Transformers

**Authors**: Ioana Gidiuta  
**Affiliations**: Department of Biomedical Engineering, University of Pennsylvania, GRASP Lab, University of Pennsylvania, Department of Electrical Engineering, University of Pennsylvania  

## Project Overview

This project aims to detect emotional and movement states in infants to enhance early detection of cerebral palsy risk through automated analysis. The project repository is organized into distinct folders for modularity and ease of use.

## Project Structure

### Main Directories

- **code_for_smaller_datasets**:  
  Contains scripts and tools optimized for smaller datasets, focusing on lightweight processing and analysis.

- **loaders**:
  - **loaders_2**:  
    A directory with the latest version of data loaders specifically for loading datasets required for emotion and movement analysis.
  - **loaders_old**:  
    Archived loaders, including:
    - `Dataloader_notebook.ipynb`: Notebook with data loading functions and utilities.
    - `Dataloader_PANDA1_PANDA3.ipynb`: Dataloader for PANDA gym datasets.
    - `Dataloader_yt.ipynb`: Loader specific to YouTube or external video datasets.

- **pipeline_for_big_datasets**:
  - **labeling_and_feature_extraction**:  
    Scripts for applying emotion classification, feature extraction, and clustering (e.g., k-means) on large datasets. Includes both successful and failed model attempts, which provide insight into various approaches.
    - `Algorithmic_emotion_classification.ipynb`: For labeling emotions in videos using pre-trained vision transformers.
    - `emotion_labels_specific_infants.ipynb`: Focuses on labeling emotions for specific infants in the dataset.
    - `k_means_with_new_features_FAILED.ipynb` and `Unsupervised_Models_FAILED.ipynb`: Unsuccessful attempts at unsupervised emotion feature extraction.
    - `Visualizer.ipynb`: For visualizing labeled emotion and movement data.
  
  - **loaders_and_dataset_creator**:  
    Contains data inspection and feature extraction scripts tailored to the PANDA gym datasets.
    - `data_inspection_and_feature_extraction_panda1_panda3.ipynb` and `data_inspection_and_feature_extraction_panda2.ipynb`: Scripts for inspecting and extracting features from PANDA datasets.
    - `dataset_creator.ipynb`: Combines different data sources into a unified format for downstream analysis.

  - **machine_learning_models**:  
    Houses models for analyzing movement and emotion data.
    - `decision_forest.ipynb`: Implements a Random Forest classifier to predict emotion labels based on extracted features.
  
- **movement_data_integration**:  
  Core integration scripts and data files for movement and emotion data, including:
  - `Movement_Data_Integration.ipynb` and `Movement_Emotion_Integration_Short_Data.ipynb`: Notebooks that integrate emotion and movement data for analysis.
  - Data files such as `Data_all_features_labeled.csv`, `Data_initial_features_labeled.csv`, and various subsets for labeled features and specific cases.

### Additional Files

- **.gitignore**:  
  Specifies files and directories to exclude from version control.
- **README.md**:  
  Project documentation (to be updated with this information).

---

This organization supports the processing pipeline for labeling, integrating, and analyzing infant emotion and movement data, all of which are central to understanding the relationship between emotional states and movement intensity in infants.