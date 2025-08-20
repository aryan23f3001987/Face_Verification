# Face_Detection

🧑‍💻 Facial Recognition App using Siamese Networks
📌 Overview

This project is a facial recognition application built using a Siamese neural network architecture, inspired directly from a research paper on one-shot learning. The Siamese model is trained to distinguish between genuine and imposter image pairs by learning an embedding space and comparing them via L1 distance.

The application itself is implemented using Kivy, providing a lightweight and interactive interface for real-time face verification through webcam input.

🚀 Key Features

Deep Learning Architecture:

Siamese neural network implemented in TensorFlow/Keras.

Custom L1 Distance layer (layers.py) for embedding similarity.

Trained to perform face verification instead of face classification.

Real-time Application:

Built with Kivy (faceid.py) for cross-platform desktop/mobile support.

Integrates with OpenCV for live webcam streaming and image capture.

Supports real-time verification against a stored set of authorized images.

Verification Pipeline:

Capture a live input image.

Preprocess (resize to 100x100, normalize).

Compare against a set of verification images.

Apply detection threshold and verification threshold to decide if the person is “Verified” or “Unverified”.

🛠️ Technologies & Tools

Deep Learning: TensorFlow, Keras

Modeling: Siamese Network with custom layers

Application: Kivy (UI), OpenCV (camera streaming)

Utilities: NumPy, OS, scikit-learn (preprocessing support)

📊 How It Works

The app captures a live frame from the webcam.

The input face is compared with stored "verification images" using the Siamese model.

For each comparison, embeddings are generated and their L1 distance is computed.

A threshold-based decision system confirms whether the person is verified.

The result is displayed dynamically on the UI (Verified ✅ or Unverified ❌).

🌍 Applications

Secure login systems

Attendance tracking

Access control in workplaces/schools

Real-time identity verification
