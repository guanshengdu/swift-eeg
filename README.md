# swift-eeg
Slow Wave Identification and Functional Tracking in EEG

# SWIFT-EEG: Slow Wave Identification and Functional Tracking in EEG

## 📌 Project Overview
SWIFT-EEG (**S**low **W**ave **I**dentification and **F**unctional **T**racking in **EEG**) is a data analysis pipeline designed to differentiate **Type I** and **Type II slow waves** based on **morphological features, neural origin, and functional properties**. The project aims to improve **EEG-based classification of slow waves** and optimize **Phase-Targeted Acoustic Stimulation (PTAS)** by leveraging machine learning, signal processing, and source localization techniques.

## 🎯 Goals
- Implement **automated slow wave detection** from high-density EEG (hdEEG).
- Compute a **synchronization score (SS)** to classify **Type I and Type II slow waves**.
- Apply **source localization techniques** to infer **subcortical vs. cortical origins** of slow waves.
- Compare slow wave properties under **PTAS and sham conditions**.
- Explore interactions between slow waves and **other sleep features** (spindles, homeostasis).

SWIFT-EEG/ │── data/ # Raw and processed EEG datasets │ ├── raw/ # Unprocessed EEG recordings │ ├── preprocessed/ # Cleaned and preprocessed EEG data │ ├── metadata/ # Subject and recording metadata │── notebooks/ # Jupyter notebooks for exploratory analysis │ ├── 01-data-preprocessing.ipynb │ ├── 02-slow-wave-detection.ipynb │ ├── 03-feature-extraction.ipynb │ ├── 04-classification.ipynb │── src/ # Source code for processing and analysis │ ├── preprocessing.py # EEG preprocessing functions │ ├── slow_wave_detection.py # Detects slow waves from EEG signals │ ├── feature_extraction.py # Extracts morphological & synchronization features │ ├── classification.py # Differentiates Type I and Type II slow waves │ ├── source_localization.py # Infers cortical and subcortical sources │ ├── visualization.py # Plots EEG waveforms and analysis results │── results/ # Output from experiments and analyses │ ├── figures/ # Plots of slow wave characteristics │ ├── statistics/ # Summarized numerical results │── scripts/ # Standalone scripts for batch processing │ ├── run_pipeline.py # Runs full data processing pipeline │── models/ # Machine learning models for classification │ ├── trained_models/ # Saved ML models │── config/ # Configuration files │ ├── settings.yaml # Experiment settings and parameters │── docs/ # Documentation files │ ├── README.md # Project documentation │ ├── methodology.md # Explanation of slow wave detection & classification │ ├── references.md # Related papers and resources │── environment.yml # Conda environment setup │── requirements.txt # Required Python packages │── .gitignore # Files to ignore in version control │── LICENSE # License information │── README.md # Project overview (this file)
