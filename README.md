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

### Model Performance

The final model used is base GPT-3.5-Turbo-1106 with zero shot prompting and has achieved the following performance metrics:


| header    | header  |
| --------- | ------- |
| Accuracy  | 90.64%  |
| Recall    | 87.50%  | 
| Precision | 60.00%  |

## License

This project is not licensed. All rights are reserved by the original authors. For permissions or licensing inquiries, please contact the Duke Law Data Lab.

## Contact

For questions or support, please contact the Duke Law Data Lab.