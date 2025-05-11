# 😄 Emotion Reader: Real-Time Emotion Detection with Emoji Overlay

This project leverages **emotion detection** in real-time through a webcam feed, using the [FER](https://github.com/priya-dwivedi/fer) library for facial emotion recognition. The application overlays an appropriate emoji on the detected face based on the recognized emotion and displays the live video feed in a graphical user interface (GUI) built with **Tkinter**.

## 🧠 Features

* 📹 **Real-time Emotion Detection** using webcam feed.
* 😊 **Emoji Overlay** on detected faces based on emotion.
* 🎥 **GUI Interface** built with Tkinter to display live video.
* 🎨 **Customizable Emojis** for different emotions.
* 🖥️ **Cross-platform compatibility** (Works on most systems with OpenCV and Tkinter).

## 😄 Supported Emotions

The emotion detector currently supports the following emotions, each mapped to a corresponding emoji:

* **Angry** → Angry emoji
* **Sad** → Sad emoji
* **Neutral** → Neutral emoji (default)

You can easily extend the emoji dictionary to support more emotions by adding new image paths for corresponding emotions.

## 🧱 Project Structure

* `main.py`: The main Python script that handles video capturing, emotion detection, and GUI rendering.
* `emojis/`: Directory containing emoji image files for each emotion.
* `requirements.txt`: List of dependencies required to run the project.

## 🚀 Installation

1. Clone the repository:

   ```bash
   git clone https://bayojuvikas/AI_Real-Time_Emotions_Reader.git
   cd AI_Real-Time_Emotions_Reader
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Make sure your webcam is connected and working.

4. Create a folder named `emojis` and place the appropriate emoji images (such as `angry.png`, `sad.png`, `neutral.png`, etc.) in it. Update the paths in the code if necessary.

## 🏃‍♂️ Running the Application

To start the emotion reader application, simply run:

```bash
python main.py
```

The webcam feed will open, and the application will begin detecting emotions, overlaying emojis on faces in real-time.

* Press the **Close** button to exit the application.

## 📦 Requirements

* Python 3.7+
* [FER library](https://github.com/priya-dwivedi/fer) for emotion detection
* [OpenCV](https://opencv.org/) for capturing webcam video
* [Pillow](https://python-pillow.org/) for image processing
* [Tkinter](https://wiki.python.org/moin/TkInter) for creating the GUI
* Required emoji images (e.g., `angry.png`, `sad.png`, `neutral.png`)

You can install the dependencies by running:

```bash
pip install opencv-python fer pillow tk
```

## 💡 How It Works

1. The webcam feed is captured using **OpenCV**.
2. The **FER** emotion detector analyzes each frame to detect facial emotions.
3. Based on the detected emotion, an emoji is selected and overlaid on the corresponding face.
4. The live video feed with overlaid emojis is displayed using **Tkinter** in a GUI.

## 📄 License

This project is licensed under the MIT License.
