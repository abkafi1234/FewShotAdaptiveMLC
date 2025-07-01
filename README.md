This project implements a multi-label hate speech classification system for Bengali text using a fine-tuned XLM-Roberta transformer model. The workflow includes:

- **Data Preparation:** Loads and preprocesses a Bengali hate speech dataset with multiple labels (e.g., Race, Gender, Religion).
- **Model Architecture:** Uses a shared XLM-Roberta encoder with task-specific heads for each label (multi-task learning).
- **Training:** First, the model is trained on all classes. Then, few-shot fine-tuning is applied to improve performance on resource-limited (low-data) classes.
- **Evaluation:** The model is evaluated using F1-score, precision, and recall, with threshold tuning for each class.
- **Few-Shot Learning:** Focuses on boosting underrepresented classes by further fine-tuning only on those samples.

The approach efficiently leverages transfer learning and few-shot fine-tuning to handle class imbalance and improve classification for minority classes.
