# Piano Difficulty Estimator

A machine learning project for estimating the difficulty of piano pieces directly from MIDI files.

The project uses the [Piano Syllabus dataset](https://zenodo.org/records/14794592) and represents each piece as a sequence of MIDI note events. A hierarchical Transformer model is trained to predict piano difficulty on a scale from **0 to 11**.

The final model achieved:

* **31.5% exact accuracy**
* **77.6% accuracy within ±1 difficulty level**
* **94.1% accuracy within ±2 difficulty levels**
* **1.01 mean absolute error**

A Random Forest model using hand-crafted MIDI features was also implemented as a baseline.

## Running the Project

The notebook was developed in **Google Colab** and can be opened directly using the Colab badge at the top of the notebook.

The dataset is downloaded automatically from Zenodo by the notebook, and the web scraping code for the rest of the data is included. Some paths are configured for Google Drive and may need to be changed before running in a different environment.

## More Information

See [`Final Report.pdf`](./Final%20Report.pdf) for a detailed description of the dataset, preprocessing pipeline, model architecture, experiments, and results.
