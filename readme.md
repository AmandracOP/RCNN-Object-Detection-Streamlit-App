## RCNN Object Detection for Marine Debris Classification with Streamlit

This project implements an R-CNN object detection model using Streamlit to distinguish between marine debris and trash in images.
Here are some sample images of how will it look like:
<div style="text-align:center">
  <p style="font-size:18px">1. Opening the website: </p>
  <img src="https://github.com/AmandracOP/RCNN-Object-Detection-Streamlit-App/assets/82217000/4e5bddb8-13b8-4e0b-83ff-b54589f62a55" alt="240628_17h44m26s_screenshot" style="width:50%;"><br>
</div>

<div style="text-align:center">
  <p style="font-size:18px">2. Adding an Image for testing from gallery: </p>
  <img src="https://github.com/AmandracOP/RCNN-Object-Detection-Streamlit-App/assets/82217000/92e9cea2-4e8b-4544-8714-ff46b1c1ce8b" alt="240629_17h48m01s_screenshot" style="width:50%;"><br>
</div>

<div style="text-align:center">
  <p style="font-size:18px">3. Model says it is a Marine: </p>
  <img src="https://github.com/AmandracOP/RCNN-Object-Detection-Streamlit-App/assets/82217000/1f242024-702b-49e8-a41a-c741c7733586" alt="240629_17h46m23s_screenshot" style="width:50%;"><br>
</div>

<div style="text-align:center">
  <p style="font-size:18px">4. Model says it is a Trash: </p>
  <img src="https://github.com/AmandracOP/RCNN-Object-Detection-Streamlit-App/assets/82217000/ad5f1fd9-e916-4017-bd58-1508ddbdf963" alt="240629_17h47m25s_screenshot" style="width:50%;"><br>
</div>

**Getting Started**

 **Clone the Repository:**
  Open your terminal and clone this repository using the following command:
   ```bash
   git clone https://github.com/AmandracOP/RCNN-Object-Detection-Streamlit-App.git
 ```

**Download the Dataset:**
The dataset used to train the model is not included in this repository due to size constraints. You can access the dataset from the following Google Drive link: \[[**Drive Link**](https://drive.google.com/drive/folders/1rdDJD8_JUetdo_3rTnKH8p-Po60amgJK?usp=drive_link)\]

Download the dataset and place it in the root directory of this project.
  
  **Update Dataset and model weights path according to your needs:**
 I assume the dataset is located in the root directory of the project. If you place it in a different location, you will need to update the path at two locations in the code:

*   line 52 model path in `app.py`
*   line 56 path definition in `rcnn_deploy.py`
*   line 91 model path in `rcnn_deploy.py`
*   line 156 model path in `rcnn_deploy.py` 

 **Create and Activate Python Virtual Environment:**
 It's recommended to create a virtual environment to isolate project dependencies. Here's an example using `venv`:
```
python -m venv venv
source venv/bin/activate  # For Linux/macOS
venv\\Scripts\\activate.bat  # For Windows
```
 **Install Dependencies:**
  Activate your virtual environment and install the required packages listed in `requirements.txt`:

```
pip install -r requirements.txt
```

 **Run the Application:**
 Start the Streamlit app by running:

```
streamlit run app.py
```

This will launch the application in your web browser, allowing you to upload images and see the model's predictions for marine debris and trash.
