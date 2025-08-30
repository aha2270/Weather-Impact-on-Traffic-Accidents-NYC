# Traffic Accident Data Analysis

## Introduction:
This project conducts an in-depth analysis of traffic accident data to uncover correlations between contributing factors and weather conditions. By merging and cleaning two seperate datasets - one containing accident details and another with corresponding weather information - this analysis aims to provide new insights into driver behavior and safety.

## Project Goal:
The primary goal of this project is to answer the following question: **What are the main factors that cause accidents and does weather play a part in accident occurance?**

The analysis explores this question by first seeing what weather conditions cause the most accidents. The next step is to analyze what contributing factors are reported the most in accidents. The final step take in the notebook is to see if there is a relationship between the weather during the accident, and what the most common contributing factor is.

## Methodology:

The analysis followed a multi-step process to prepare and analyze the data:

  1. **Data Merging**: Two seperate datasets were merged into a single DataFrame using a common unique identifier to link each accident to its corresponding weather information.
  2. **Data Consolidation**: The raw weather data, which included numerous specific descriptions (e.g., 'Rain: Heavy', 'Snow: Light', 'Clear sky'), was consolidated into three core bins: **Rain, Snowy**, and **Clear/Cloudy**
  3. **Data Filtering**: The merged and cleaned dataset was filtered to isolate accidents where the primary **Contributing Factor** was **Driver Inattention/Distraction**
  4. **Visualization**: Multiple visualizations were created to explore the data, culminating in a bar chart that compares the number of "Driver Inattention/Distraction" accidents across the three weather bins. This final visual provides a clear representation of the key findings.

## Key Findings:
The visual analysis of the data revealed several compelling insights:
 - **Driver caution is a factor**: There were significantly fewer distracted driving accidents in snowy weather conditions compared to rainy or clear conditions. This suggests that deivers may be more attentive and cautious when faced with the precieved danger of snow
 - **Rainy weather may be underestimated**: Suprisingly, the analysis showed that more distracted driving accidents occurred during rainy conditions than in clear conditions. This indicates that while drivers may know the dangers of rain, they may be underestimating its impact or not adapting their behavior as much as they do in snow

## How to Run the Code:
To replicate this analysis, ensure you have Python installed, along with the necessary libraries.

**Prerequisites**:
 - `Pandas`
 - `numpy`
 - `requests`
 - `matplotlib`
 - `seaborn`
 - `scipy`

You can install these using pip:

`pip install pandas numpy requests matploylib seaborn scripy`

**Instructions**
  1. Open the `Weather-Impact-Analysis.ipynb` file in a Jupyter Notebook enviornment (e.g., JupyterLab, VS Code, Google Colab).
  2. Run the cells sequentially to execute the data processing and visualization steps.
  3. The final bar chart will be displayed within the notebook output

### Project Files
 - `Weather-Impact-Analysis.ipynb`: The main Jupyter Notebook file for data processing and visualization
 - `README.md`: This file.
