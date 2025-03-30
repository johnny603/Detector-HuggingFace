#  Detect Banana with Hugging Face

A simple web application that uses Hugging Face's image classification models to determine if an image contains a banana or not
Shoutout to codedex.io for guiding me in this project

##  Description

This project implements a web interface where users can upload an image, and the application will classify whether the image contains a hotdog. It leverages pre-trained image classification models from Hugging Face's model hub to perform the detection.

##  Features

- Upload images through a user-friendly web interface
- Real-time classification using Hugging Face's image recognition model
- Visual feedback on whether the uploaded image contains a hotdog
- Mobile-responsive design

## Technologies Used

- Python
- Flask (web framework)
- Hugging Face Transformers (for image classification)
- HTML/CSS/JavaScript (frontend)
- Bootstrap (responsive styling)

## 📦 Installation

1. Clone this repository
2. Open in your desired IDE of choice (this was made in PyCharm by the creator)
3. Create and activate a virtual environment:
   ```
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. Install dependencies:
   ```
   python -m pip install flask
   pip install python-dotenv
   pip install requests
   ```

## 🔧 Usage

1. Create a .env file
2. Shortcut:
```
touch .env
```
3. Initialize API variables
```
HUGGING_FACE_API_URL=HUGGING_FACE_API_URL=https://api-inference.huggingface.co/models/andrewvanbeek/autotrain-not-something-2133568871
HUGGING_FACE_API_KEY=your_key_here
```
4. Log into huggingface.co and create a API key
5. Start the Flask application:
   ```
   python3 web.py
   ```
6. Open the first link on the console in a web browser
7. Upload an image using the interface
8. The application will analyze the image and tell you if it's a banana or not!

## How It Works

The application uses a pre-trained image classification model from Hugging Face to analyze uploaded images. When you upload an image, the application:

1. Processes the image to fit the model's requirements
2. Sends the processed image to the model
3. Receives classification probabilities for different objects
4. Checks if "banana" is one of the top predictions
5. Displays the result to the user

## Learning Outcomes

By building this project, you'll learn about:
- Implementing machine learning models in web applications
- Working with the Hugging Face Transformers library
- Creating a responsive web interface for ML applications
- Processing and analyzing image data

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements

- Uses models from [Hugging Face](https://huggingface.co/)
- Project idea from [Codedex.io](https://www.codedex.io/projects/detect-hotdog-with-hugging-face)
