NLP projects

---

In the A1 folder there is the pdf report of the project and the notebook.  
The notebook aims to categorize the sexist messages according to the intention of the author in one of the following categories: direct sexist message, reported sexist message and judgemental message.   
Topics:  
- Data Cleaning
- Text Encoding
- Model definition-training-evaluation (Bidirectional LSTM)
- Transformers finetuning-training-evaluation ([Twitter-roBERTa-base for Hate Speech Detection](https://huggingface.co/cardiffnlp/twitter-roberta-base-hate))
- Error Analysis

---

In the A2 foler there is the pdf report of the project and the notebook.  
The notebook aims to label the sentence as not-sexist or one of these four sexist categories:   
(1) threats,  
(2)  derogation,  
(3) animosity,  
(4) prejudiced discussion.   
To classify them we use only propting tecniques (few-shot) using the following models:   
- [Mistral v3](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.3)
- [Llama v3.1](https://huggingface.co/meta-llama/Llama-3.1-8B-Instruct)
- [Qwen3](https://huggingface.co/Qwen/Qwen3-1.7B)    
Topics: 
- Prompt setup
- Inference
- Few-shot inference
- Evaluation/Error Analysis
