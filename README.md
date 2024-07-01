# Classification of Private Letter Rulings (PLRs) using LLMs

## Overview

This project leverages prompt engineering and fine-tuning of large language models (LLMs) to classify Private Letter Rulings (PLRs) into Adverse and Non-Adverse rulings. It is designed to aid legal professionals in quickly and accurately categorizing PLRs.

## Repository Structure

- **`data/`**: Contains datasets used for training and testing the model.
- **`src/`**: Source code for data processing, prompt engineering, model fine-tuning, and inference.
- **`requirements.txt`**: List of dependencies required to run the project.

## Installation

Clone the repository using HTTPS:

```bash
git clone https://gitlab.oit.duke.edu/duke-law-datalab/plr_chatgpt.git
```

Navigate to the project directory:

```bash
cd plr_chatgpt
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Usage

### Data Preparation

Place your PLR data files in the `data/` directory.

### Training the Model

To train the model, run the following command:

```bash
python src/train_model.py --data_dir data/ --output_dir models/
```

### Inference

To classify new PLRs, use the inference script:

```bash
python src/infer.py --model_dir models/ --input_file data/new_plrs.csv --output_file results/classified_plrs.csv
```

## License

This project is not licensed. All rights are reserved by the original authors. For permissions or licensing inquiries, please contact the Duke Law Data Lab.

## Contact

For questions or support, please contact the Duke Law Data Lab.