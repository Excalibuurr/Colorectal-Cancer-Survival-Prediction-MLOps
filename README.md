# Colorectal Cancer Survival Prediction MLOps

This repository provides an end-to-end MLOps pipeline for predicting colorectal cancer survival using machine learning techniques. It incorporates model training, data processing, Kubeflow pipeline integration, and a web application for predictions.

## Project Structure

- **application.py**: Flask web application serving predictions for colorectal cancer survival. Loads pre-trained model and scaler, renders the homepage, and provides a `/predict` endpoint that takes user input and returns survival predictions.
- **kubeflow_pipeline/**: Contains Kubeflow pipeline components and initialization files for orchestrating ML workflows.
- **notebook/notebook.ipynb**: Jupyter notebook for exploratory data analysis, model development, and experimentation.
- **src/**: Core source code.
    - `custom_exception.py`: Custom exception handling for robust error management.
    - `data_processing.py`: Functions and classes for preprocessing and transforming data.
    - `logger.py`: Logging utilities for tracking pipeline events and errors.
    - `model_training.py`: Scripts for training machine learning models.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Excalibuurr/Colorectal-Cancer-Survival-Prediction-MLOps.git
    cd Colorectal-Cancer-Survival-Prediction-MLOps
    ```
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

- **Run the web application**:
    ```bash
    python application.py
    ```
    Access the dashboard at [localhost:5000](http://localhost:5000).

- **Kubeflow Pipeline**: Refer to the `kubeflow_pipeline` directory for instructions on running the pipeline components.

- **Jupyter Notebook**:
    ```bash
    jupyter notebook notebook/notebook.ipynb
    ```
    Use the notebook for model experimentation and analysis.

## Contributing

Feel free to open issues or pull requests for improvements or new features.

## License

This project is licensed under the MIT License.

## Acknowledgments

This project utilizes Kubeflow, Flask, scikit-learn, and related open-source technologies for building scalable and reproducible ML workflows.
