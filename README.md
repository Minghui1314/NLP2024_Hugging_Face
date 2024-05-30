# NLP2024_Hugging_Face
IMDB Sentiment Classifier

This is an IMDB movie review sentiment classifier based on the DistilBERT model. It is trained using Hugging Face's Transformers library and the model is uploaded to the Hugging Face model library.

 How to run the code

1. Install the necessary libraries:
   !pip install transformers datasets huggingface_hub
2. Run the code in the Jupyter Notebook file to complete data processing, model training, and evaluation.
3. Upload the trained model to Hugging Face:
Ensure you have set up your Hugging Face account and created a model repository. Use the provided code snippet in the notebook to upload the model.
Example Code Snippet for Uploading to Hugging Face

from huggingface_hub import notebook_login, HfApi

notebook_login()

api = HfApi()
repo_name = "imdb-sentiment-classifier"  
api.upload_folder(
    folder_path="./my_model",
    repo_id=f"Minghui131/{repo_name}",  
    repo_type="model"
)
