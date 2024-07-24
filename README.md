# Social Media Toxicity Moderation
This project aims to revolutionize Social Media Toxicity Moderation by leveraging the capabilities of LLAMA-2 7B with 4-bit quantization. Utilizing a Kaggle dataset of labeled Wikipedia comments, the project focuses on six categories of toxicity: toxic, severe_toxic, obscene, threat, insult, and identity_hate. Given the rise of digital communication, this dataset is essential for understanding and predicting toxic behavior in user-generated content. The resulting classification model helps automate the identification and moderation of harmful content, promoting a safer and more inclusive online community.

# Model Choice
Apart from being open-source, LLAMA-2 was chosen for its robust performance across diverse benchmarks, consistently surpassing other LLMs in accuracy and effectiveness. Its Parameter-Efficient Fine-Tuning (PEFT) capabilities, utilizing QLORA and SFT Trainer, streamline the fine-tuning process by reducing the number of parameters requiring updates and quantizing the weights. This efficiency accelerates training times and reduces computational costs, making LLAMA-2 a resource-efficient option for researchers and developers.

# Results
The fine-tuned model demonstrated exceptional performance, with high accuracy, F1 scores, precision, and recall, especially in handling imbalanced data. The ROC curves indicated consistent performance between 85% and 95% across all classes. While the model excelled overall, the threat classification performance highlighted an area for improvement due to limited training examples. Increasing data for minority classes and further training can optimize the model's capabilities, promising even better results in future iterations.

![confusion_matrix](Confusion_matrix.png)

# Future Research Directions
Future research could explore Mixture of Experts (MoE) models, like Mixtral 8x7b a scaled-down version of GPT-4 with 8 experts, each handling specialized sub-tasks. This efficient architecture reduces parameters while maintaining a comparable context size. Applying MoE techniques could enhance the efficiency and accuracy of text classification tasks, particularly for challenging datasets like toxicity classification.
