# README

## English to Hindi Machine Translation using Hugging Face

This project performs **English → Hindi machine translation** using a Hugging Face model and evaluates the translations using **BLEU**, **chrF**, and **TER** metrics.

---

## Requirements

* Python 3.10 or later
* pip
* Internet connection (to download the Hugging Face model)

---

## Install Dependencies

Install all required packages using:

```bash
pip install pandas transformers torch sentencepiece accelerate sacrebleu openpyxl
```

---

## Project Structure

```
project/
│
├── Assignment_1.pynb
├── Assignment_2.pynb
├── README.md

and output results

```

---

## Input Dataset

The input dataset should contain at least the following columns:

* `english`
* `hindi`

Example:

| english      | hindi        |
| ------------ | ------------ |
| Hello        | नमस्ते       |
| How are you? | आप कैसे हैं? |

---

## Running the Program

Open a google colab and run 
Note : add a secret api key as HF_TOKEN in your google colab securities tab from hugging face 

```bash
Assignment_1.pynb
```


```bash
Assignment_2.pynb
```

---

## Output

After execution, the program generates:

```bash
cleaned_dataset.xlsx
```
  * Original English sentences
  * Reference Hindi translations
  * Predicted Hindi translations


```bash
translation_metrics.txt
```
  * BLEU Score
  * chrF Score
  * TER Score

---

## Hugging Face Model

Example model used:

```
facebook/nllb-200-distilled-600M
```

The model will be downloaded automatically during the first execution and cached locally. Subsequent runs will use the cached model.

---

## Notes

* A GPU is recommended for faster translation but is not required.
* The first execution may take longer because the model needs to be downloaded.
* Ensure that the input dataset is correctly formatted before running the program.

---

## Author

Diptesh Karmakar
