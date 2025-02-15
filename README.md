# SWIFT-EEG: Slow Wave Identification and Functional Tracking in EEG

## 📌 Project Overview
SWIFT-EEG (**S**low **W**ave **I**dentification and **F**unctional **T**racking in **EEG**) is a data analysis pipeline designed to differentiate **Type I** and **Type II slow waves** based on **morphological features, neural origin, and functional properties**. The project aims to improve **EEG-based classification of slow waves** and optimize **Phase-Targeted Acoustic Stimulation (PTAS)** by leveraging machine learning, signal processing, and source localization techniques.

## 🎯 Goals
- Implement **automated slow wave detection** from high-density EEG (hdEEG).
- Compute a **synchronization score (SS)** to classify **Type I and Type II slow waves**.
- Apply **source localization techniques** to infer **subcortical vs. cortical origins** of slow waves.
- Compare slow wave properties under **PTAS and sham conditions**.
- Explore interactions between slow waves and **other sleep features** (spindles, homeostasis).

## 📂 Folder Structure
SWIFT-EEG/
│── data/                     # Raw and processed EEG datasets
│   ├── raw/                  # Unprocessed EEG recordings
│   ├── preprocessed/         # Cleaned and preprocessed EEG data
│   ├── metadata/             # Subject and recording metadata
│
│── notebooks/                # Jupyter notebooks for exploratory analysis
│   ├── 01-data-preprocessing.ipynb   # Data cleaning & filtering
│   ├── 02-slow-wave-detection.ipynb  # Slow wave event detection
│   ├── 03-feature-extraction.ipynb   # Extracting SW features
│   ├── 04-classification.ipynb       # Classification of SW types
│
│── src/                      # Source code for processing and analysis
│   ├── preprocessing.py       # EEG preprocessing functions
│   ├── slow_wave_detection.py # Detects slow waves from EEG signals
│   ├── feature_extraction.py  # Extracts morphological & synchronization features
│   ├── classification.py      # Differentiates Type I and Type II slow waves
│   ├── source_localization.py # Infers cortical and subcortical sources
│   ├── visualization.py       # Plots EEG waveforms and analysis results
│
│── results/                  # Output from experiments and analyses
│   ├── figures/              # Plots of slow wave characteristics
│   ├── statistics/           # Summarized numerical results
│
│── scripts/                  # Standalone scripts for batch processing
│   ├── run_pipeline.py       # Runs full data processing pipeline
│
│── models/                   # Machine learning models for classification
│   ├── trained_models/       # Saved ML models
│
│── config/                   # Configuration files
│   ├── settings.yaml         # Experiment settings and parameters
│
│── docs/                     # Documentation files
│   ├── README.md             # Project documentation
│   ├── methodology.md        # Explanation of slow wave detection & classification
│   ├── references.md         # Related papers and resources
│
│── environment.yml           # Conda environment setup
│── requirements.txt          # Required Python packages
│── .gitignore                # Files to ignore in version control
│── LICENSE                   # License information
│── README.md                 # Project overview (this file)

## 📊 Data Processing Workflow
1. **Preprocessing:**  
   - Bandpass filtering (0.5–4 Hz)
   - Artifact removal (ICA, bad channel detection)
   - Epoch segmentation

2. **Slow Wave Detection:**  
   - Identifies slow waves using amplitude and slope thresholds
   - Extracts peak-to-peak amplitude, duration, and number of negative peaks

3. **Feature Extraction:**  
   - Computes **synchronization score (SS)**
   - Extracts **phase, frequency, and spatial distribution** of slow waves

4. **Classification:**  
   - Differentiates **Type I** (widespread, subcortico-cortical) and **Type II** (local, cortico-cortical) slow waves

5. **Source Localization:**  
   - Uses **sLORETA/eLORETA** for cortical source reconstruction

## 🔬 Research Relevance
This project contributes to **sleep science, neurotechnology, and cognitive research** by improving:
- **EEG-based sleep staging**
- **PTAS (Phase-Targeted Acoustic Stimulation) precision**
- **Memory consolidation studies**
- **Clinical applications for insomnia and depression treatment**

## 📚 References
- Siclari et al., 2014. *Two Distinct Synchronization Processes in the Transition to Sleep: Evidence from High-Density EEG*.  
- Bernardi et al., 2018. *Spontaneous sleep slow wave detection and functional characterization*.  
- Murphy et al., 2009. *Source modeling of sleep slow waves*.  

## 📢 Contributing
Contributions are welcome! Please open an issue or submit a pull request if you have improvements or bug fixes.


### **Explanation of Folder Structure:**
- **`data/`**: Stores raw, preprocessed EEG data and metadata.
- **`notebooks/`**: Contains Jupyter notebooks for interactive data analysis.
- **`src/`**: Core Python scripts for EEG processing, feature extraction, classification, and visualization.
- **`results/`**: Stores outputs such as figures and statistics from experiments.
- **`scripts/`**: Standalone scripts for batch processing.
- **`models/`**: Stores trained ML models for slow wave classification.
- **`config/`**: Configuration files for experiment settings.
- **`docs/`**: Documentation for methodology and references.



