# Financial Sentiment Analysis
**Introduction**

In this project, I built LSTM and bidirectional LSTM models to classify headlines and other financial texts into three labels: negative, neutral, and positive. The goal is to capture subtle wording and provide clearer signals for studying how news and disclosures relate to stock-price movements.

**Dataset**

The dataset contains financial-domain sentences collected from two resources: the FiQA dataset and the Financial PhraseBank accessed via Kaggle. The corpus consists of thousands of short text samples, each annotated for sentiment  as positive, negative, or neutral. 
The dataset contains 5,322 unique sentences comprising a total of 122,710 words. Each entry represents a financial text sample written in English.

**Implementation Details**

<img src="Model architecture/ModelArchitecture.jpg" alt="Model Architecture" width="400">

**Results**

This shows an example of correctly classified sentiment along with the accuracy score.

Text: [According to the Finnish russian chamber of commerce all the major construction company of Finland are operating in Russia ] 
LSTM model  results:
Predicted label: positive. True label: positive (97.62%)
Bidirectional LSTM model results
 Predicted label: positive . True label: positive (99.89%)

<img width="592" height="325" alt="image" src="https://github.com/user-attachments/assets/9afc8eac-33e0-4649-bfeb-6c3bbafa1643" />
<img width="533" height="427" alt="image" src="https://github.com/user-attachments/assets/124c3cfe-74ba-4a82-b5c4-5a6b37166873" />

**Conclusion**

This project shows that the LSTM model can provide solid accuracy and adding a bidirectional layer to the LSTM model can slightly improve the accuracy scores. However, both models performed well on the sentiment analysis task.

- Limitations 
The limitation of this project include the models’ potential difficulty in handling contextual dependencies.

- Future Scope
This project may be further improved by fine-tuning domain models such as FinBERT and other Transformers, which provide contextual representations better suited to financial language. 

**References**

[1] C. Shah, A Hands-On Introduction to Machine Learning. Cambridge: Cambridge University Press, 2022.
[2] D. Jurafsky and J. H. Martin, "Deep Learning Architectures for Sequence Processing," in Speech and Language Processing, 3rd ed., Stanford University, ch. 9. [Online]. Available: https://web.stanford.edu/~jurafsky/slp3/9.pdf.
[3] S. Ganguli et al., "Reverse-engineering recurrent networks for sentiment classification reveals line attractor dynamics," arXiv preprint, 2019. [Online]. Available: https://ganguli-gang.stanford.edu/pdf/19.ReverseEng.pdf

