Project Title
Deepfake Audio Detection

Description
This project focuses on detecting deepfake audio generated using advanced AI techniques such as speech synthesis, voice conversion, and replay attacks. Deepfake audio poses significant risks to security systems, especially in domains like banking, customer service, and law enforcement. The project leverages state-of-the-art deep learning models, including Long Short-Term Memory (LSTM) networks, Convolutional Neural Networks (CNNs), and Generative Adversarial Networks (GANs), to identify and classify synthetic audio. The solution emphasizes the use of transfer learning and feature extraction techniques for robust detection.

Features
Deep Learning Models: Utilizes LSTM, CNNs, and GANs for detection.

Feature Extraction: Employs techniques like spectrograms, Mel-Frequency Cepstral Coefficients (MFCCs), spectral centroid, spectral bandwidth, and zero-crossing rate.

Dataset Handling: Preprocessing pipelines for cleaning, feature extraction, and dataset splitting.

Transfer Learning: Incorporates transfer learning principles to improve detection performance.

Evaluation Metrics: Uses metrics like F1-score and tandem decision cost function (t-DCF) for model evaluation.

Dataset
The project uses the ASVspoof 2019 dataset (https://datashare.ed.ac.uk/handle/10283/853), a benchmark dataset for automatic speaker verification spoofing detection. It includes:

Logical Access (LA) scenarios: Text-to-speech (TTS) and voice conversion (VC) attacks.

Physical Access (PA) scenarios: Replay attacks under controlled acoustic conditions.

The dataset is divided into training, validation, and test sets:

Training: 17,615 samples

Validation: 5,413 samples

Testing: 3,212 samples

Other datasets referenced include the RFP dataset and FakeAVCeleb dataset.

Methodology
Data Preprocessing
Feature Extraction:

Spectrograms

MFCCs (Mel-Frequency Cepstral Coefficients)

Chroma STFT

Spectral Centroid

Spectral Bandwidth

Zero Crossing Rate

Data Splitting:

Training Set

Validation Set

Test Set

Normalization:
Standardized features to ensure consistency across samples.

Model Training
Implemented deep learning models with PyTorch to classify audio as real or fake. Key steps include:

Loading data using custom datasets.

Training on extracted features with LSTM and CNN architectures.

Evaluating performance using cross-validation.

Evaluation Metrics
F1-score

Tandem Decision Cost Function (t-DCF)

Results
The models achieved high accuracy on the ASVspoof 2019 dataset but exhibited challenges in generalizing to external datasets. Future work aims to address these limitations through domain adaptation techniques and multimodal learning approaches.

Future Directions
Domain Adaptation: Improve generalizability across datasets by employing techniques like noise injection, pitch shifting, and speed variation.

Multimodal Learning: Combine audio data with video or text for enhanced detection accuracy.

Self-Supervised Learning: Leverage models like Wav2Vec 2.0 and HuBERT for robust feature representation.

Graph Neural Networks (GNNs): Explore relationships among diverse audio features for better detection.

Quantum Computing: Investigate quantum systems for computationally intensive tasks in deepfake detection.


Contributors
Kavya Verma

Ojas Kulkarni

Sagnik Samanta

Kabit Gulati

Divyanshi Mittal

Muzaffar Ahmad Dar

C.L. Biji

License
This project is licensed under the MIT License.
