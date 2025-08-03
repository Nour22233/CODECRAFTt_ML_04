🧠 Hand Gesture Recognition - CodeCraft Task 04

This project is a real-time hand gesture recognition system using a CNN model trained on the LeapGestRecog dataset.Each recognized gesture triggers a specific action on the computer (e.g., open YouTube, take a screenshot, control volume, etc.).

📁 Dataset:

Dataset used: LeapGestRecog

The dataset includes 10 gesture classes:

['Palm', 'L', 'Fist', 'Fist_moved', 'Thumb', 'Index', 'Ok', 'Palm_moved', 'C', 'Down']

🛠 Install dependencies:

pip install opencv-python numpy tensorflow keras pyautogui

▶️ Run the code:

Make sure you have the trained model file named gesture_cnn_model.h5 in the same directory.

Then run the main script:

python gesture_control.py

The webcam will open and recognize gestures in real-time.

🧩 Gesture-to-Action Mapping

Gesture

Action

Palm

Open Calculator

L

Open YouTube

Fist

Volume Up

Fist_moved

Volume Down

Thumb

Take Screenshot

Index

Open Google

Ok

Close Google Chrome

Palm_moved

Open Jupyter Notebook

C

Mute System Volume

Down

Pause for 1 second (cooldown)

⏱️ Cooldown Between Actions

To avoid repeated execution of the same command, there's a 1-second cooldown between gesture detections.

🧪 Model

The model used is a CNN trained on grayscale 64x64 gesture images.

Input shape: (64, 64, 1)

Loss: categorical_crossentropy

Optimizer: Adam

Accuracy achieved: ~98% on test set

📷 Example (Optional)

You can add screenshots or demo GIFs showing the webcam interface + triggered actions here.

📦 Structure

.
├── gesture_control.py         # Main gesture detection script
├── gesture_cnn_model.h5       # Trained model file
├── README.md                  # Project documentation
└── utils/                     # (optional) helper functions, if any

👩‍💻 Author

Made with nour hesham for CodeCraft Task 04

