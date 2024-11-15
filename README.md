# Week 3 Headstarter Accelerator Project 3 Brain Tumor Classification with Neural Networks
Week 3: Brain Tumor Classification with Neural Networks.
In this project, you will learn how to train neural networks to classify tumors in brain MRI scans. You will learn about how to construct different neural network architectures through transfer learning and custom convolutional layers, and use the Gemini 1.5 Flash model to generate explanations for the model's predictions.
[Link to Brain Tumor MRI Dataset on Kaggle](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset).
## About Dataset: Brain Tumor MRI Dataset, a dataset for classify brain tumors
### What is a brain tumor?
A brain tumor is a collection, or mass, of abnormal cells in your brain. Your skull, which encloses your brain, is very rigid. Any growth inside such a restricted space can cause problems. Brain tumors can be cancerous (malignant) or noncancerous (benign). When benign or malignant tumors grow, they can cause the pressure inside your skull to increase. This can cause brain damage, and it can be life-threatening.
### The importance of the subject
Early detection and classification of brain tumors is an important research domain in the field of medical imaging and accordingly helps in selecting the most convenient treatment method to save patients life therefore.

## Step for run
You can run this [*Week_3_Headstarter_Accelerator_Project_3_Brain_Tumor_Classification_with_Neural_Networks.ipynb*]() in your Google Colab account (or you can run in jupyter notebook local, kaggle notebook and so on).
If you don't have GPU ram memory in your Google Colab: first run [*Week_3_Headstarter_Accelerator_Project_3_Brain_Tumor_Classification_with_Neural_Networks.ipynb*](), download your ```xception_model.weights.h5``` and ```cnn_model.h5``` (also you can do more files like ```.h5``` for web app), upload to your Google Drive (or storage like Google Drive) and second acces your files from Google Drive use to Google Colab [*Week_3_Headstarter_Accelerator_Project_3_Brain_Tumor_Classification_with_Neural_Networks.ipynb*]()

## Web application with streamlit
I use Ngrok api key for web application with streamlit and I run in Google Colab the web application with streamlit.
The web application utilizes the following machine learning models for tumor prediction:
- **Transfer Learning**
- **Xception**
- **Custom CNN**
- **you can use other Deep Learning models like**: **ResNet50**, **various customs CNNs**, **EfficientNet**, **MobileNet**, **VGG19** and so on.

In the Google Colab notebooks in GitHub, you don't see this completely for web application with streamlit:

```python

st.write("## Classification Results")

    result_container = st.container()
    result_container = st.container()

    result_container.markdown(
    f"""
    <div style="background-color: #000000; color: #ffffff; padding: 30px; border-radius: 15px;">
        <div style="display: flex; justify-content: space-between; align-items: center;">
            <div style="flex: 1; text-align: center;">
                <h3 style="color: #ffffff; margin-bottom: 10px; font-size: 20px;">Prediction</h3>
                <p style="font-size: 36px; font-weight: 800; color: #FF0000; margin: 0;">
                    {result}
                </p>
            </div>
            <div style="width: 2px; height: 80px; background-color: #ffffff; margin: 0 20px;"></div>
            <div style="flex: 1; text-align: center;">
                <h3 style="color: #ffffff; margin-bottom: 10px; font-size: 20px;">Confidence</h3>
                <p style="font-size: 36px; font-weight: 800; color: #2196F3; margin: 0;">
                    {prediction[0][class_index]:.4%}
                </p>
            </div>
        </div>
    </div>
    """,
    unsafe_allow_html=True
    )

```

## Resources

- [**Kaggle Dataset**](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)

- [**What is a Neural Network?**](https://www.youtube.com/watch?v=aircAruvnKk)

- [**How Neural Networks Learn**](https://www.youtube.com/watch?v=IHZwWFHWa-w)

- [**What is a Convolution**](https://www.youtube.com/watch?v=KuXjwB4LzSA)

- [**Interactive CNN Explainer**](https://poloclub.github.io/cnn-explainer/)

- [**How Tesla uses Neural Networks to Power Self Driving**](https://www.youtube.com/watch?v=FnFksQo-yEY)

- [**What is Transfer Learning**](https://builtin.com/data-science/transfer-learning)

- [**Saliency Map Implementation**](https://medium.com/@bijil.subhash/explainable-ai-saliency-maps-89098e230100)









