# Evaluating Hugging Face Models on NorEval with Google Colab 🇳🇴🤖

This repository provides a Google Colab notebook designed to easily evaluate Hugging Face language models (e.g., Google's Gemma 3, Mistral, Llama) on tasks from the **NorEval benchmark**.

I'm very excited about NorEval, a benchmark recently released by the Language Technology Group (LTG) at the University of Oslo! It signifies a major step forward for NLP research in Norwegian, offering the most comprehensive evaluation suite for both Bokmål and Nynorsk. This tool is invaluable for anyone researching or developing LLM-based applications in Norwegian.

This Colab notebook aims to demonstrate how NorEval can be used to benchmark state-of-the-art open-source LLMs, such as Google's Gemma 3 models. I hope this example helps bridge the gap between cutting-edge language models and specialized Norwegian language evaluation.

---

## About NorEval

NorEval, developed by the Language Technology Group at the University of Oslo, is a benchmark for evaluating Norwegian language models.

**Key Features of NorEval**:
* Comprises **24 high-quality human-created datasets** across **9 task categories**.
* Covers tasks like sentiment analysis, Norwegian language knowledge, commonsense reasoning, machine translation, and text summarization.
* Establishes **human baselines**.
* Integrates over **100 carefully designed prompts**.
* Supports both **Bokmål and Nynorsk**.

---

## 🚀 The Colab Notebook: Easy NorEval Evaluation

This project provides a Colab notebook that allows researchers and practitioners to easily evaluate models like Google's Gemma 3 on NorEval tasks. The notebook utilizes the `lm-evaluation-harness` for running the evaluations.

* **Access the Colab Notebook:** [https://colab.research.google.com/drive/1Fq89q2GtgZQlZcA3FYGTW5GhhdO50mVm](https://colab.research.google.com/drive/1Fq89q2GtgZQlZcA3FYGTW5GhhdO50mVm)

### How To Use the Notebook:

1.  **Prerequisites**:
    * A Hugging Face Account.
    * A Hugging Face Access Token (`read` role) for gated models (like Gemma, Llama 3).
    * Accept terms of use on the Hugging Face page for any gated models.
    * Use a GPU runtime in Colab (T4 GPU or better recommended).
2.  **Install Dependencies**:
    * Execute "Step 1: Install Dependencies" in the Colab notebook.
3.  **Setup Hugging Face Authentication (if needed)**:
    * Run "Step 2: Setup Hugging Face Authentication" and add your `HF_TOKEN` to Colab's Secrets Manager.
4.  **Clone NorEval Repository**:
    * Execute "Step 3: Clone NorEval Repository" to download task configurations.
5.  **Configure and Run Evaluation**:
    * In "Step 4: Configure and Run Evaluation...", select your Hugging Face Model ID, NorEval Task(s), and adjust other settings (precision, quantization, few-shot, batch size, output directory).
    * Run the cell. This can take a significant amount of time.
6.  **(Optional) View Raw Output Files**:
    * Run "Step 5: View Raw Output Files (Optional)" to list generated files.
7.  **Analyze Results**:
    * Run "Step 6: Analyze and Present Results" to load metrics and display them in a summary table.

---

## 🔗 Key Links & Resources

* **NorEval Paper:** [https://arxiv.org/pdf/2504.07749](https://arxiv.org/pdf/2504.07749) (from Colab) or [https://lnkd.in/dp8UsBdv](https://lnkd.in/dp8UsBdv)
* **NorEval GitHub Repository (LTG Oslo):** [https://github.com/ltgoslo/noreval](https://github.com/ltgoslo/noreval)
* **Evaluation Colab Notebook:** [https://colab.research.google.com/drive/1Fq89q2GtgZQlZcA3FYGTW5GhhdO50mVm?usp=sharing](https://colab.research.google.com/drive/1Fq89q2GtgZQlZcA3FYGTW5GhhdO50mVm?usp=sharing)
* **Example Model Tested (Gemma 3 1b it):** [https://huggingface.co/google/gemma-3-1b-it](https://huggingface.co/google/gemma-3-1b-it)

---

## ❤️ Acknowledgements

Amazing work by the authors of NorEval: **Vladislav Mikhailov, Tita Enstad, David Samuel, Hans Christian Farsethås, Andrey Kutuzov, Erik Velldal, and Lilja Øvrelid**. This is truly an outstanding contribution to Norwegian NLP research and a vital tool for advancing AI in Norwegian. Their work will undoubtedly accelerate progress in developing more capable and better-aligned language models for the Norwegian language.

---

If you are interested in Norwegian language technology or multilingual NLP, I encourage you to explore these resources and contribute to extending them to different domains.
