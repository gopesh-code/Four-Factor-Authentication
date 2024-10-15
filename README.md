
# Four Factor Authentication using AI

## Overview

This project aims to enhance the security of web-based applications by implementing a **Four-Factor Authentication** system. The method incorporates traditional authentication factors and biometric techniques, powered by Artificial Intelligence (AI). The four factors include:

1. **Password Verification**
2. **Email-OTP Verification**
3. **Face Recognition**
4. **Speech Recognition-enabled Security Question**

This multi-layered security approach significantly reduces the chances of unauthorized access while maintaining user convenience.

## Features

- **Password Authentication**: Standard alphanumeric password-based authentication.
- **Email-based OTP Verification**: A one-time password (OTP) is sent to the user's registered email for verification.
- **Facial Recognition**: Utilizes computer vision techniques for identity verification based on facial features.
- **Speech Recognition**: Employs speech-to-text APIs for answering security questions, adding an additional voice biometric layer.
  
## Technologies Used

- **Python**: The core language for backend logic.
- **Dlib**: A library used for face recognition.
- **SpeechRecognition API**: To handle speech input for security questions.
- **Flask**: For web framework and server-side management.
- **HTML/CSS**: Front-end UI design.
- **SQLite**: Local database for user data storage.

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/gopesh-code/Four-Factor-Authentication.git
   cd Four-Factor-Authentication
   ```

2. **Set up virtual environment**:
   ```bash
   python -m venv env
   source env/bin/activate  # For Windows: env\Scripts\activate
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up the database**:
   The application uses SQLite for user data storage. Ensure that the `myData.db` file is present or create a new one using the provided schema.

5. **Run the application**:
   ```bash
   python server.py
   ```

6. **Access the web interface**:
   Open a browser and go to `http://localhost:5000`.

## Usage

- **Sign Up**: Users can sign up by providing basic details, including their face and voice samples.
- **Login**: 
   1. Enter your password.
   2. Verify OTP sent to your email.
   3. Perform face recognition through the webcam.
   4. Answer a security question through voice recognition.

## File Structure

```plaintext
├── app/                   # Main application logic
├── static/                # Static files (CSS, JS, images)
├── templates/             # HTML templates for front-end
├── voice_db/              # Voice data files for speech recognition
├── face_recog_dlib_file/   # Face recognition model files
├── requirements.txt       # Dependencies
├── server.py              # Flask server
└── README.md              # This file
```

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
