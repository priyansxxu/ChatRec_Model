ChatRec_Model is an offline conversational AI system built using a fine-tuned GPT-2 Transformer.
It predicts User A's next response based on the conversational context provided, enabling context-aware and human-like dialogue generation.
ChatRec_Model/
 ChatRec_Model.ipynb      : Main Jupyter Notebook (data preprocessing, training & evaluation)
 Report.pdf               : Technical report summarizing model design, training, and results
 Model.joblib             : Serialized fine-tuned GPT-2 model and tokenizer
 ReadMe.txt               : Documentation (this file)
Install Dependencies:
  pip install torch transformers datasets nltk rouge-score sacrebleu pandas scikit-learn joblib tqdm

Add data Set

