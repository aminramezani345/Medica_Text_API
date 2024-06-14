# AJAA App for Sleep Parameters Extraction

This project is a Streamlit web application designed to process medical notes to extract and summarize sleep parameters using pre-trained NLP models.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Models](#models)
- [Contributing](#contributing)
- [License](#license)

## Features
- Summarizes medical notes using a pre-trained T5 model.
- Extracts specific sleep parameters using a pre-trained DistilBERT model fine-tuned for question answering.

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/ajaa-app.git
    cd ajaa-app
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Ensure you have the pre-trained models saved in the `Models` directory. You can download them from Hugging Face or any other source and place them in the appropriate subdirectories (`t5_base` for summarization and `distilbert-base-cased-distilled-squad` for question-answering).

## Usage
1. Run the Streamlit app:
    ```bash
    streamlit run main.py
    ```

2. Open your web browser and go to `http://localhost:8501` to view and interact with the application.

## Project Structure
- `main.py`: The main script that runs the Streamlit web application.
- `Models/`: Directory containing the pre-trained models.
  - `t5_base/`: Directory containing the T5 model for summarization.
  - `distilbert-base-cased-distilled-squad/`: Directory containing the DistilBERT model for question-answering.
- `requirements.txt`: List of dependencies required for the project.

## Models
- **Summarization Model**: T5 base model for summarization tasks.
- **Question Answering Model**: DistilBERT model fine-tuned on the SQuAD dataset for extracting answers from text.

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request or open an issue for any bugs or feature requests.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
