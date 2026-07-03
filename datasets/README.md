# Datasets

This directory contains information about accessing the datasets used for training and evaluating the ML models.

## Dataset Storage

Due to file size limitations on GitHub, datasets are stored on **Google Drive**. Please use the link below to access them:

### 📁 [Access Datasets on Google Drive](https://drive.google.com/YOUR-DRIVE-LINK-HERE)

## Dataset Types

- **Rayleigh Fading**: Empirical channel measurements with Rayleigh fading characteristics
- **3GPP CDL**: Industry-standard 3GPP Clustered Delay Line channel models
- **DeepMIMO (OpenCSI)**: Advanced large-scale MIMO channel dataset

## Drive Folder Structure

```
datasets/
├── rayleigh_fading/          # Rayleigh channel measurements
├── 3gpp_cdl/                 # 3GPP CDL channel data
└── deepmimo_opencsi/         # DeepMIMO dataset files
```

## Usage

To use datasets:

1. Visit the Google Drive link above
2. Download the dataset files you need
3. Place them in the corresponding local `datasets/` subdirectories
4. Reference dataset paths in your notebooks and training scripts
5. Ensure proper data preprocessing before model training

## Download Instructions

- Right-click on files/folders and select "Download"
- For large folders, create a shortcut or download as ZIP
- Extract files to your local project directory

---

**Note**: Contact the repository maintainer if you need access permissions to the Google Drive folder.
