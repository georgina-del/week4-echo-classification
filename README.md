# Week 4 - Echo Classification (Sea Leads vs Sea Ice)


## Project Overview
This project applies **unsupervised learning methods** to classify Sentinel-3 altimetry echos into **sea ice** and **sea ice leads**. The analysis extracts waveform features and evaluates the clustering results against the official ESA surface classification.  

The main goal is to demonstrate how unsupervised methods can automatically separate different surface types in polar regions without prior labels.


---


## Built With
- **Python 3.11** – main programming language  
- **Google Colab** – notebook environment  
- **NumPy** – numerical computations  
- **Matplotlib** – plotting and visualization  
- **scikit-learn** – K-means and Gaussian Mixture Model (GMM)  
- **rasterio** – reading Sentinel-2 optical bands  
- **netCDF4** – reading Sentinel-3 altimetry data


---


## Getting Started

### Prerequisites
Make sure you have access to the GEOL0069 AI for Earth Observation Jupyter Notebook (link can be found on the Moodle page)

Download the workbook and additional data via the week 4 Jupyter Notebook

Make sure you have a Google Drive and Google Collab account set up and can access these workspaces

or Python 3.7+ installed, plus the libraries listed above. You can install them using:
```bash
pip install numpy matplotlib scikit-learn rasterio netCDF4
```

---

### How to Run
1. Open the notebook `Unit_2_Unsupervised_Learning_Methods.ipynb` in **Google Colab**.  
2. Mount your Google Drive to access the data files.
3. Edit file paths where necessary.
4. Run all cells.  

> Optional: If you prefer, you can clone this repository locally:
> ```bash
> git clone https://github.com/your_username/week4-echo-classification.git
> ```


---


## Usage
- The notebook performs the following tasks:
1. Loads and preprocesses Sentinel-3 altimetry data.
2. Extracts key waveform features: sig0, peakiness (PP), and stack standard deviation (SSD).
3. Runs Gaussian Mixture Model (GMM) clustering to classify echoes into two clusters.
4. Computes the mean echo waveform and standard deviation for each class.
5. Compares clustering predictions to ESA labels using a confusion matrix and classification report.
6. Visualizes results using scatter plots and echo plots.


---

## Roadmap
- Add K-means comparison with GMM
- Include additional visualizations for waveform alignment
- Extend to Sentinel-2 optical imagery classification

---


## Contributing
Contributions to improve the clarity of explanations, code annotation, or visualizations are welcome. To contribute:
1. Fork the repository
2. Create a feature branch: git checkout -b feature/AmazingFeature
3. Commit your changes: git commit -m "Add AmazingFeature"
4. Push to branch: git push origin feature/AmazingFeature
5. Open a pull request

---


## License
Distributed under the Unlicense License. See LICENSE.txt for details.


---


### Contact
Georgina Ruber
Email: georgina.ruber.25@ucl.ac.uk
GitHub: https://github.com/your_username/week4-echo-classification


---

## Acknowledgments
ESA Sentinel-3 & Sentinel-2 data
Dr Michel Tsamados course content 
Dr Michel Tsamados and Weibin Chen Jupyter Notebook
scikit-learn documentation
Matplotlib documentation



