# Publishing GPT2 Version #3

#### Models Stored Here: https://drive.google.com/drive/folders/1D65R81woux6nYjDHG-kdhjg085cbp4U4?usp=sharing

## Text Generation Model - Proof of Concept
This repository contains a proof of concept for a text generation model designed to emulate the writing style of specific authors. By training a GPT-2 model on selected texts, the model generates new text resembling the author's tone, style, and structure when provided with a user-defined prompt.

## Project Overview
This project demonstrates:

- Fine-tuning a pre-trained language model to mimic the style of well-known authors.
- Using prompts to guide the generation of custom text in the desired style.
- Leveraging openly available classic literature for training data.

### Technologies Used
- Python: The primary programming language.
- Transformers Library: Used for fine-tuning GPT-2.
- PyTorch and TensorFlow: For model training and conversion.
- Hugging Face Datasets: To manage and preprocess the text data.
- Project Gutenberg: Source of literary texts for training data.

### Model Architecture
- Base Model: GPT-2, a transformer-based language model, fine-tuned for specific author styles.
- Tokenizer: GPT-2 tokenizer with additional tokens to mark the beginning and end of author-specific texts.
- Fine-Tuning: Pre-trained GPT-2 is further trained on datasets created by preprocessing texts from Project Gutenberg. This includes texts by:
    - Arthur Conan Doyle
    - Charles Dickens
    - Mary Shelley

The fine-tuned model generates text by appending user prompts and generating characters until a specified limit is reached.

## Sources and Resources
- Project Gutenberg: Public domain books used for training. Examples include:
  - Arthur Conan Doyle: A Study in Scarlet, The Adventures of Sherlock Holmes, The Sign of Four, etc.
  - Charles Dickens: A Christmas Carol, Great Expectations, etc.
  - Mary Shelley: Frankenstein, The Last Man, etc.
- Transformers Library: Hugging Face Transformers
- Datasets: Hugging Face Datasets

## How to Use
1. Setup: Install the necessary libraries:  

    `pip install transformers torch tensorflow datasets`

2. Training:  
    - Specify the author, number of books to train on, a prompt, and the desired character count.
    - Preprocess the selected texts and fine-tune GPT-2.

3. Text Generation:  
    - Input a prompt and generate text up to the specified character limit.
    - Save the generated text to a file for further use.


## Improvements and Future Directions
- Expanded Author Base: Include more authors to broaden the scope of stylistic emulation.
- Enhanced Text Preprocessing: Improve the preprocessing pipeline to retain more stylistic nuances.
- Advanced Architectures: Explore newer models like GPT-3 or GPT-4 for better performance.
- Evaluation Metrics: Develop objective metrics to measure how well the generated text aligns with the author's style.
- Interactive Interface: Create a web-based or command-line interface for easier user interaction.

## License  
This project uses texts from the Project Gutenberg collection, which are in the public domain. The code is open-source and free to use under the MIT License.  

Feel free to explore, experiment, and contribute to this project!  
