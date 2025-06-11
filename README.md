#Next Word Prediction Using LSTM

## Project Overview

This project implements a deep learning model to predict the **next word in a given text sequence** using **LSTM (Long Short-Term Memory)** networks. It leverages the rich and challenging text of Shakespeare's *Hamlet* to train a model capable of understanding language structure and predicting contextually accurate words.

---

## Workflow

### 1️.Data Collection

* **Dataset**: Text of *Hamlet* by William Shakespeare
* **Source**: [Project Gutenberg](https://www.gutenberg.org/ebooks/1524)

### 2️.Data Preprocessing

* Tokenize the text
* Create sequences from the tokens
* Pad sequences to uniform length
* Split into training and testing datasets

### 3️.Model Building

* **Layers**:

  * Embedding layer
  * Two stacked LSTM layers
  * Dense output layer with **Softmax** activation
* **Framework**: [TensorFlow](https://www.tensorflow.org/) + [Keras](https://keras.io/)

### 4️.Model Training

* Use training data to fit the model
* Implement **EarlyStopping** to prevent overfitting

### 5️.Model Evaluation

* Evaluate the model using sample sentences
* Predict the next word and compare it to actual next words

### 6️.Deployment

* A web app built using **[Streamlit](https://streamlit.io/)**
* User can enter a sequence of words and get predicted next word in real-time


## Tech Stack & Resources

| Tool/Library       | Purpose                            |
| ------------------ | ---------------------------------- |
| Python             | Programming Language               |
| TensorFlow + Keras | Deep Learning Model Implementation |
| NLTK / re          | Text Preprocessing                 |
| Streamlit          | Web App Deployment                 |
| NumPy / Pandas     | Data Handling and Transformation   |

### 📚 Resources Used:

* [Shakespeare's Hamlet - Project Gutenberg](https://www.gutenberg.org/ebooks/1524)
* [TensorFlow Documentation](https://www.tensorflow.org/)
* [Streamlit Docs](https://docs.streamlit.io/)
* [Keras Sequential API](https://keras.io/guides/sequential_model/)
* [NLTK Tokenizer](https://www.nltk.org/)

---

## Sample Usage

```bash
# To run the Streamlit app:
streamlit run app.py
```

In the web interface, type:

> "To be, or not to"

And the model may predict:

> **"be"**

---

## Author

**Aditya Chine**
🔗 [LinkedIn](https://www.linkedin.com/in/aditya-chine001/)
🐱 [GitHub](https://github.com/adityachine)

---

## Future Improvements

* Fine-tune on larger datasets (e.g., Wikipedia corpus)
* Implement Transformer-based prediction
* Enable multi-word prediction
* Add speech-to-text interface for input

---

## License

This project is open-sourced under the MIT License. See the `LICENSE` file for more details.
