🍅 Tomato Leaf Disease Detection & Classification
This repository contains a specialized Deep Learning solution for identifying various tomato plant pathologies. Developed as part of a Computer Engineering project, it focuses on creating a high-performance model that remains computationally efficient and resource-aware.

🌟 Features
Multi-Class Detection: Engineered to recognize multiple tomato health states (e.g., Bacterial Spot, Early Blight, Late Blight, Yellow Leaf Curl, and Healthy).

Optimized Architecture: Utilizes a custom Convolutional Neural Network (CNN) optimized for high spatial feature extraction with minimal parameter overhead.

Resource-Constrained Training: Specifically tuned to handle RAM limitations by utilizing a streamlined data augmentation pipeline.

Data Pipeline Efficiency: Employs tf.data API with prefetching and caching to maximize GPU utilization and minimize CPU bottlenecks.

Green AI Principles: Focused on reducing the carbon footprint of training by utilizing efficient resizing and early-stopping mechanisms.

📊 Model Performance
Accuracy: Achieved a robust validation accuracy (approx. 98%) across all target classes.

Validation: Verified using categorical cross-entropy loss and accuracy metrics to ensure real-world reliability.

📁 Project Structure
Bash
tomato-disease-detection/
├── notebook/
│   └── training.ipynb   # Core training logic, EDA, and model evaluation
├── models/              # Exported model files (.h5 / .keras)
├── .gitignore
└── README.md
🛠️ Technical Stack
Framework: TensorFlow / Keras

Libraries: NumPy, Pandas, Matplotlib, OpenCV

Environment: Jupyter Notebook / Google Colab

⚙️ Implementation Details
1. Preprocessing & Resizing
To manage computational load, all images are standardized to 256x256 pixels. This specific resolution was chosen to balance the preservation of fine disease textures (like small fungal spots) with the need for memory efficiency.

2. Strategic Data Augmentation
Due to RAM exhaustion challenges during development, a "Few-but-Effective" augmentation strategy was implemented:

Random Horizontal/Vertical Flips: To account for different camera orientations in the field.

Random Rotation: To ensure the model recognizes leaf patterns from any angle.

Note: These are applied "on-the-fly" during training to keep the memory footprint low.

🗺️ Future Enhancements
API Integration: Wrapping the model in a FastAPI backend for real-time web inference.

Quantization: Converting the model to TensorFlow Lite (TFLite) for offline mobile deployment in rural areas.

Edge Integration: Deploying on IoT-enabled cameras for automated greenhouse monitoring.

👨‍💻 Author
Sandeep

GitHub: @sandeepdgn
