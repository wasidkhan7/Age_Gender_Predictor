# Age_Gender_Predictor

# Age and Gender Classification with UTKFace Dataset

This project uses a ResNet50 + finetunning  to predict **age** and **gender** from face images using the [UTKFace Dataset](https://susanqq.github.io/UTKFace/).

###  Dataset
- [UTKFace Dataset Download Link](https://susanqq.github.io/UTKFace/)
- Contains 20k+ facial images labeled with age, gender, and ethnicity.

###  Tools Used
- Python
- TensorFlow / Keras
- OpenCV
- Google Colab
- Flask (for web UI)
- VS Code (for editing)
- GitHub (for version control)

###  How it works
- We used a pretrained ResNet model + fine_tuned it  on facial images to classify **gender** (binary classification) and **age** (as regression or class).
- Due to hardware limitations (low RAM, no GPU), the **age prediction** model is a bit biased and less accurate.
- The **gender prediction** model works quite well.

###  Colab Notebook
- Run the notebook in [Google Colab](https://colab.research.google.com/)
- You can upload your image using the upload cell.
- The model predicts your **age** and **gender** instantly.

###  Limitations
- Age prediction model is little biased due to underfitting on a small system, instead of 2300 imgs i worked on 4000 imgs .
- GPU or Colab Pro recommended for better training but didnot upport at all .

###  Metric          | Result                                   
| --------------- | --------------------------------------       |
| Gender Accuracy |  Good (\~85%+)                               |
| Age MAE         | GOOD but Biased due to low resource training |
| Training Device | Colab (GPU Enabled)                          |


###  Future Work
- Improve model architecture
- Train for longer on Colab or Kaggle
- Deploy on Streamlit or Flask for real-time web inference

###  Author
- Wasid Khan

