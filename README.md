# 🌍 Hyperspectral Change Detection Based on Spectral Unmixing

This project leverages hyperspectral imaging and spectral unmixing techniques to detect subtle environmental changes over time. By applying the Linear Mixing Model (LMM), we decompose mixed pixel spectra into pure material signatures (endmembers) and their corresponding abundances, enabling more precise land cover analysis.

## 🧪 Objective

To develop an automated system for detecting land surface changes using hyperspectral remote sensing data, improving upon the limitations of traditional pixel-based methods.

## 📌 Key Features

- **Spectral Unmixing**: Implementation of the Linear Mixing Model (LMM) to separate mixed spectral signatures into constituent endmembers and abundance maps.
- **Change Detection**: Identification of temporal environmental changes using abundance differences across hyperspectral images.
- **Preprocessing**: Includes noise removal, band selection, normalization, and alignment of temporal datasets.
- **Visualization**: Heatmaps and difference maps to highlight areas with significant spectral variation.

## 🧠 Techniques & Tools

- **Linear Mixing Model (LMM)**
- **Spectral Angle Mapper (SAM)**
- **Image Preprocessing and Denoising**
- **Principal Component Analysis (PCA)** (optional for dimensionality reduction)

## 🛠 Tech Stack

- **Languages**: Python, MATLAB
- **Libraries/Packages**:
  - `numpy`, `scipy`, `matplotlib`
  - `spectral` (for hyperspectral image processing)
  - MATLAB Image Processing Toolbox
- **Data Sources**: AVIRIS/NASA open hyperspectral datasets or simulated hyperspectral cubes

## 🚀 How It Works

1. **Data Acquisition**: Load hyperspectral image cubes (pre- and post-change).
2. **Preprocessing**: Perform noise reduction, bad band removal, and normalization.
3. **Spectral Unmixing**:
   - Extract endmembers using N-FINDR or VCA (Vertex Component Analysis).
   - Calculate abundance maps via Fully Constrained Least Squares (FCLS).
4. **Change Detection**:
   - Compare abundance maps to locate spectral changes.
   - Visualize and quantify land cover modifications.

## 📁 Project Structure

Hyperspectral-Change-Detection/
│
├── data/ # Sample hyperspectral datasets
│
├── python_code/ # Scripts for spectral unmixing and visualization
│ ├── unmixing.py
│ ├── change_detection.py
│ └── utils.py
│
├── matlab_code/ # Optional MATLAB implementations
│ └── spectral_unmixing.m
│
├── results/ # Output abundance maps and difference images
│
└── README.md
