# Classification of Private Letter Rulings (PLRs) using LLMs

## Overview

This project leverages prompt engineering and fine-tuning of large language models (LLMs) to classify Private Letter Rulings (PLRs) into Adverse and Non-Adverse rulings. It is designed to aid legal professionals in quickly and accurately categorizing PLRs.

## Repository Structure

- **`data/`**: Contains datasets used for training and testing the model.
- **`src/`**: Source code for data processing, prompt engineering, model fine-tuning, and inference.
- **`environment_setup_testing.ipynb`**: This notebook will help you set up the environment, install the required dependencies, and test the environment.
- **`requirements.txt`**: List of dependencies required to run the project.

_Note_: All notebooks have a summary at the top outlining what the notebook achieves and the purpose it serves.<br>
_Note_: All the PLRs have been scraped from the IRS and can be found in `data/raw/files_definite_plr`.

## Before you get started

Make sure you have the following:
- OpenAI API key. You can sign up [here](https://auth.openai.com/authorize?issuer=auth0.openai.com&client_id=DRivsnm2Mu42T3KOpqdtwB3NYviHYzwD&audience=https%3A%2F%2Fapi.openai.com%2Fv1&redirect_uri=https%3A%2F%2Fplatform.openai.com%2Fauth%2Fcallback&device_id=547004bc-0db1-4b5d-b83d-25e0e7ad616d&scope=openid+profile+email+offline_access&response_type=code&response_mode=query&state=SnlCbX5vNVRHeUt4QktBenZxMnBLUHF0ZUVTSFExTmctZ1UwTk1WckUxeA%3D%3D&nonce=NHZDflhELmxUeDJVbi42RjNwMnVLa0tHRH5MYm5JWUVWM2ZZeGV3U21xcA%3D%3D&code_challenge=cfAS5H1VuvJXSYf7hN_jxjU4m-UaEjWPcdKe8N7HWuU&code_challenge_method=S256&auth0Client=eyJuYW1lIjoiYXV0aDAtc3BhLWpzIiwidmVyc2lvbiI6IjEuMjEuMCJ9&flow=control) and get free $5 credits.

## Installation and Reproducing our project

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

Run our scripts:
_Note_: Before running the scripts in the src/ folder, please set up the environment with the help of the environment_setup_testing.ipynb notebook.

```bash
cd src
```

1. Use prod_by_year.ipynb to generate classifications of PLRs by year or a list of years.
2. Fine_tuning.ipynb can be used to prepare the training dataset for fine-tuning the model and evaluate model performance.

## Usage

### Model Performance

The final model used is base GPT-3.5-Turbo-1106 with zero shot prompting and has achieved the following performance metrics:


| Metric    | Value   |
| --------- | ------- |
| Accuracy  | 90.64%  |
| Recall    | 87.50%  | 
| Precision | 60.00%  |

## License

This project is not licensed. All rights are reserved by the original authors. For permissions or licensing inquiries, please contact the Duke Law Data Lab.

## Contact

For questions or support, please contact the Duke Law Data Lab.