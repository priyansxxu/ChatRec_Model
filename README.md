ChatRec_Model is an offline conversational AI system built using a fine-tuned GPT-2 Transformer.
It predicts User A's next response based on the conversational context provided, enabling context-aware and human-like dialogue generation.
ChatRec_Model/
 ChatRec_Model.ipynb      : Main Jupyter Notebook (data preprocessing, training & evaluation)
 Report.pdf               : Technical report summarizing model design, training, and results
 Model.joblib             : Serialized fine-tuned GPT-2 model and tokenizer
 
Install Dependencies:
  pip install torch transformers datasets nltk rouge-score sacrebleu pandas scikit-learn joblib tqdm

2. Place your conversation dataset (conversationfile.xlsx or .csv) in the working directory.

3. Run ChatRec_Model.ipynb to preprocess, train, and evaluate the model.

4. After training:
   - The model will be saved as ./final_model/ (Hugging Face format)
   - It will also be serialized as ChatRec_Model/Model.joblib

----------------------------------------------------------
Evaluation Summary
----------------------------------------------------------
BLEU Score : 0.0102
ROUGE-1    : 0.1500
ROUGE-2    : 0.0000
ROUGE-L    : 0.1000
Perplexity : 53.9670

----------------------------------------------------------
Model Justification
----------------------------------------------------------
Model  : GPT-2 (autoregressive Transformer)
Reason : Efficient for small datasets, capable of context-aware text generation.
Deployment : Joblib serialization allows fast loading in production (Flask/FastAPI).

----------------------------------------------------------
Author's Note
----------------------------------------------------------
This model serves as a prototype. For production, train with more data and consider
larger models (GPT-2 Medium, T5, or Longformer) for better context understanding.


model Link: https://drive.google.com/file/d/1YtWJRZnqS0vWwlGF3Qq2ZhEutRge8Mub/view?usp=drive_link

