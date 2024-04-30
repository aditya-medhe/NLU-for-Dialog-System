

# Conversational AI Chatbot

This repository contains code for a conversational AI chatbot that utilizes Natural Language Understanding (NLU) techniques such as intent recognition, entity extraction, slot filling, and context handling. The chatbot is implemented using Python and the following libraries:

- `scikit-learn` for intent classification using RandomForestClassifier
- `spaCy` for named entity recognition (NER)
- `transformers` library for BERT fine-tuning for intent recognition
- `torch` for deep learning model training and inference
- `tkinter` for building the GUI

## Setup Instructions

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/your-username/conversational-ai-chatbot.git
   ```

2. Navigate to the project directory:

   ```bash
   cd conversational-ai-chatbot
   ```

3. Install the required dependencies using pip:

   ```bash
   pip install -r requirements.txt
   ```

4. Download the spaCy English language model:

   ```bash
   python -m spacy download en_core_web_sm
   ```

5. Download the pre-trained BERT model using the `transformers` library:

   ```bash
   python -c "from transformers import BertTokenizer, BertForSequenceClassification; BertTokenizer.from_pretrained('bert-base-uncased'); BertForSequenceClassification.from_pretrained('bert-base-uncased')"
   ```

## Usage

To run the chatbot, simply execute the `gui_app.py` script:

```bash
python gui_app.py
```

This will open a GUI window where you can interact with the chatbot by entering text queries. The chatbot will perform intent recognition, entity extraction, slot filling, and context handling, and display the generated response.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to customize the README.md file according to your project's specifics and add any additional sections or information as needed.
