# face_expression_recognition_pytorch
PyTorch CNN implementation of Face Expression Recognition Dataset from Kaggle.

Dataset: https://www.kaggle.com/jonathanoheix/face-expression-recognition-dataset

Class Distribution:
Angry : 3993
Disgust: 436
Fear: 4103
Happy: 7164
Neutral: 4982
Sad: 4938
Surprise: 3205

Model Architecture:
Conv1 [Conv (o/p: 512, 48, 48), BatchNorm, ReLU, MaxPool (o/p: 512, 24, 24)]
Conv2 [Conv (o/p: 128, 24, 24), BatchNorm, ReLU, MaxPool (o/p: 128, 12, 12)]
Conv3 [Conv (o/p: 64, 12, 12), BatchNorm, ReLU, MaxPool (o/p: 64, 6, 6)]
Conv4 [Conv (o/p: 64, 6, 6), BatchNorm, ReLU, MaxPool (o/p: 256, 3, 3)]
Fully Connected Layer (i/p: 256*3*3, o/p: 7)

Learning Rate: 0.001
Optimizer: Adam
Epochs: 5

