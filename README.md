# Fig2Num: A Tool for Automated Data Extraction from Bar Chart Figures

## Authors

- **Jun Kong**  
  Department of Mathematics and Statistics, Georgia State University, Atlanta, GA, USA  
  Email: jkong@gsu.edu

- **Kenji Mizumoto**  
  Graduate School of Advanced Integrated Studies in Human Survivability, Kyoto University, Japan  

- **George Teodoro**  
  Department of Computer Science, Federal University of Minas Gerais, Brazil
  
- **Gerardo Chowell**  
  Department of Population Health Sciences, School of Public Health, Georgia State University, Atlanta, GA, USA  
  Email: gchowell@gsu.edu

## Purpose

Fig2Num is a MATLAB-based tool designed to efficiently and accurately extract data from bar chart figures. This tool is particularly useful for researchers in epidemiology and other fields where data may only be available in graphical form. Fig2Num automates the process of extracting numerical data from bar charts, reducing the time and effort required for manual data extraction and minimizing the risk of errors.

For example, prediction of outbreaks and spatial spread of infectious diseases highly depends on accurately collecting and integrating large-scale epidemic data from multiple resources. However, such data are often demonstrated in bar chart figures published in a format where original data can be readily used. As a result, the capability to extract such data from bar charts in an automated fashion becomes the key to enabling ensuing prediction analysis. We develop tool for efficient and accurate data extraction from bar chart figures. The developed conversion method leverages the power of image analysis and only requires minor manual intervention, enabling analysis in a batch mode for large-scale data conversion.

## Features

- **Automated Data Extraction**: Efficiently extracts data from bar charts, including complex figures like stacked bar charts with multiple colors.
- **User-Friendly**: Minimal user input required with step-by-step instructions and visual guides for ease of use.
- **High Accuracy**: Proven reliability with validation against simulated and real-world epidemic data.
- **Flexible Output**: Extracted data is saved in a format conducive to further analysis and visualization.
- **Visual Validation**: Tools for comparing extracted data with the original figures to ensure accuracy.

## Getting Started

### Prerequisites

- MATLAB 2018a or later
- Image Processing Toolbox

### Installation
1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/gchowell/Fig2Num.git


# Usage

(1)
```bash
# extract data from a bar chart in style 1:
figure2num_clean(data_path, filename, result_path)
```
e.g.
```bash
figure2num_clean('../data/', 'figure1_20190808.png', '../result/')
```

(2)
```bash
# extract data from a bar chart in style 2:
figure2num_DRC(data_path, filename, dates, result_path)
```
e.g.
```bash
figure2num_DRC('../data/', 'SITREP_EVD_DRC_20191126-eng.png', [2018 4 30 2019 11 18], '../result/')
```

(3)
```bash
# extract data from a bar chart in style 3 (i.e. in grouped style):
figure2num_group(data_path, filename, dates, result_path)
```
e.g.
```bash
figure2num_group('../data/', 'nejmsr_fig4.tiff', [2018 8 1 2019 5 1], '../result/')
```


## Contributing

Contributions to Fig2Num are welcome! If you have suggestions for improvements or new features, please open an issue or submit a pull request. See the `CONTRIBUTING.md` file for more information.
