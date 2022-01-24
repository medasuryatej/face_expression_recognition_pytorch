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

Model Architecture: <br/>
Conv1 [Conv (o/p: 512, 48, 48), BatchNorm, ReLU, MaxPool (o/p: 512, 24, 24)] <br/>
Conv2 [Conv (o/p: 128, 24, 24), BatchNorm, ReLU, MaxPool (o/p: 128, 12, 12)] <br/>
Conv3 [Conv (o/p: 64, 12, 12), BatchNorm, ReLU, MaxPool (o/p: 64, 6, 6)] <br/>
Conv4 [Conv (o/p: 64, 6, 6), BatchNorm, ReLU, MaxPool (o/p: 256, 3, 3)] <br/>
Fully Connected Layer (i/p: 256*3*3, o/p: 7) <br/>

Learning Rate: 0.001 <br/>
Optimizer: Adam <br/>
Epochs: 5 <br/>

