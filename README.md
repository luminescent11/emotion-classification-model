# emotion-classification-model
The notebook for my emotion-classification-api model, using a frozen HuBERT feature extractor and feeding it into a classifier head. Achieves 79% test accuracy. [Link for the Google Colab (identical notebook)](https://colab.research.google.com/drive/1vFuc-dgZgUlzi1ZlMuFjrZaZBYHACZNC)

You can find the data [here](https://www.kaggle.com/datasets/uldisvalainis/audio-emotions?resource=download-directory). For this notebook to work, you either have to set up your drive like below, or configure data_path to match where Emotions API Data is. Have the raw data stored in the Emotions folder, with subfolders for each emotion **there's a typo in the Kaggle dataset, so rename the "suprised" folder to "surprised"**. Don't worry about the Resampled folder, the notebook will create it when preprocessing the data.

Your data_path will be different depending on whether you are running this notebook on Google Colab or locally.

MyDrive/ -> Emotions API Data/ -> Emotions/, Resampled/

Example reconfiguration:
data_path = "project_root/data"

project_root/ -> data/ -> Emotions/, Resampled/
