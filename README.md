# Enhanced YouTube Comment Analysis

## Overview
The **Enhanced YouTube Comment Analysis** project aims to classify YouTube comments into six categories:  
- Appreciation  
- Normal  
- Trolling  
- Suggestions  
- Questions  
- Other Languages  

This project not only provides detailed classification but also summarizes important questions and suggestions to enhance insights. It leverages **machine learning techniques** with a Random Forest classifier and integrates **Generative AI** for generating summaries. The front-end is implemented as a YouTube-like interface to display categorized comments.

---

## Features
- **Comment Classification**: Detects and categorizes comments into six emotional or functional groups.
- **Multi-language Support**: Works with English and Hinglish comments, detecting non-supported languages.
- **Generative AI-powered Summary**: Provides a concise summary of key questions and suggestions to highlight actionable insights.
- **Front-end UI**: A YouTube-clone interface that displays categorized comments.
- **Scalable Back-end**: Model deployed using Flask for real-time predictions.
  
---

## Project Architecture
1. **Data Collection**  
   - YouTube Data API used to retrieve comments from various videos.  
   - Additional data from Kaggle’s YouTube dataset for model enhancement.  

2. **Data Preprocessing and Feature Engineering**  
   - Cleaned and preprocessed the dataset to remove duplicates and handle missing values.  
   - TF-IDF vectorization used to convert text into numerical features.  

3. **Model Training**  
   - Random Forest Classifier used for prediction due to its robustness and high accuracy (91.71%).  
   - Dataset split into 80% training and 20% testing.

4. **Back-end and Front-end Integration**  
   - Flask framework used to serve the model through API endpoints.  
   - UI built to mimic YouTube, showing categorized comments with summaries.

---

## Tech Stack
- **Languages**: Python  
- **Libraries**: NumPy, Pandas, Scikit-Learn, NLTK, Flask, Pickle  
- **APIs**: YouTube Data API  
- **Front-end**: HTML, CSS  
- **Deployment**: Flask Server  

---

## How to Run Locally
1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/Enhanced-YouTube-Comment-Analysis.git
   cd Enhanced-YouTube-Comment-Analysis
   ```

2. **Install Dependencies**  
   Make sure you have Python installed. Then, run:
   ```bash
   pip install -r requirements.txt
   ```

3. **Obtain YouTube API Key**  
   - Create a project on [Google Cloud Console](https://console.cloud.google.com/).
   - Enable the YouTube Data API and generate an API key.
   - Add the API key in the appropriate file (e.g., `config.py`).

4. **Train the Model (Optional)**
   If you want to retrain the model, run:
   ```bash
   python train_model.py
   ```

5. **Run the Flask Server**
   ```bash
   python app.py
   ```

6. **Access the Application**  
   Open your browser and navigate to:  
   ```
   http://127.0.0.1:5000/
   ```


---

## Screenshots
### 1. Front-end YouTube Clone Interface  
- Displays categorized comments with predicted labels.
- ![result 1](https://github.com/user-attachments/assets/83627ced-6df0-4027-9a53-1cb3af29f58f)
 

### 2. Summary Section  
- Shows the most important questions and suggestions extracted from user comments.
- ![WhatsApp Image 2024-10-16 at 21 25 26_e59da6ff](https://github.com/user-attachments/assets/bb27b0a1-d60e-43f4-8ce3-554cb888c10b)

- 

---

## Future Enhancements
- Adding support for more languages.
- Implementing advanced NLP techniques like BERT for better accuracy.
- Enabling more interactive visualizations on the front-end.

---

## License
This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

---


- Open for contributions! Feel free to submit a pull request.
