# AI Image Classifier (1000 Classes)

Welcome to the **AI Image Classifier**, a modern, dark-themed desktop application built with Python. This tool leverages the power of **PyTorch** and the **ResNet-18** architecture to identify objects across 1,000 different ImageNet categories. Whether you have a single mystery photo or a massive folder of vacation snapshots, this app has the "vision" to sort them out.

<img width="1920" height="1032" alt="Στιγμιότυπο οθόνης 2026-04-29 181554" src="https://github.com/user-attachments/assets/4d694a83-37ac-43d1-8c77-bc18027501aa" />


---

## 🚀 Features

* **Real-Time Inference:** Fast classification using a pre-trained ResNet-18 model.
* **Batch Processing:** Point the app at a folder, and it will churn through every image, providing a progress bar and a calculated **ETA**.
* **Modern UI:** A sleek, macOS-inspired dark interface featuring "Inter" typography and elevated card layouts.
* **Live Preview:** See exactly what the AI is looking at as it processes files.
* **Detailed Logging:** A scrollable activity log that tracks top-k predictions and confidence scores.

---

## 🛠️ Technical Stack

| Component | Technology |
| :--- | :--- |
| **Language** | Python 3.x |
| **Deep Learning** | PyTorch & Torchvision |
| **UI Framework** | Tkinter (with Custom TTK Styling) |
| **Image Handling** | Pillow (PIL) |
| **Model** | ResNet-18 (Pre-trained on ImageNet) |

---

## 📥 Installation

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/yourusername/ai-image-classifier.git
    cd ai-image-classifier
    ```

2.  **Install Dependencies:**
    Make sure you have `torch`, `torchvision`, and `Pillow` installed.
    ```bash
    pip install torch torchvision pillow
    ```

3.  **Run the App:**
    ```bash
    python main.py
    ```
    *(Note: On first run, the app will automatically download the ResNet-18 weights and the ImageNet label mapping file.)*

---

## 🖥️ How to Use

### Single Image Classification
1.  Click **Browse** to select an image from your computer.
2.  Hit **Classify**.
3.  The top 5 predictions and their percentage confidence will appear in the log.

### Folder Classification
1.  Click **Choose...** to select a directory containing multiple images.
2.  Click **Classify Folder**.
3.  Sit back and watch the **Progress Bar**. The app will calculate the **ETA** based on your hardware's processing speed.

<img width="1920" height="1032" alt="Στιγμιότυπο οθόνης 2026-04-29 181612" src="https://github.com/user-attachments/assets/558975e4-92ab-44b0-99db-5c4f5d3aadf0" />


---

## 🧠 Model Details
The application uses **ResNet-18**, a convolutional neural network that is 18 layers deep. It treats images by:
* Resizing them to $224 \times 224$ pixels.
* Normalizing them based on the ImageNet mean and standard deviation.
* Applying a **Softmax** function to the final layer to turn raw scores into human-readable probabilities.

> **Note:** Performance may vary depending on whether you are running this on a CPU or GPU. By default, the script is configured for standard compatibility.

---

## 🎨 UI Preview
The interface is designed for clarity and focus:
* **Left Panel:** High-resolution preview and a technical activity log.
* **Right Panel:** Control center for file selection and batch operations.
* **Bottom Bar:** Real-time status updates (e.g., "Loading model," "Idle," "Classifying").

---

## ⚖️ License
This project is open-source. Feel free to fork it, break it, or improve it! 

*Happy classifying! If the AI thinks your cat is a "Space Shuttle," maybe it's just telling you your cat is out of this world.* 🐱🚀
