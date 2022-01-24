# face_expression_recognition_pytorch
PyTorch CNN implementation of Face Expression Recognition Dataset from Kaggle.

Dataset: https://www.kaggle.com/jonathanoheix/face-expression-recognition-dataset

Class Distribution: <br/>
Angry : 3993 <br/>
Disgust: 436 <br/>
Fear: 4103 <br/>
Happy: 7164 <br/>
Neutral: 4982 <br/>
Sad: 4938 <br/>
Surprise: 3205 <br/>

![class_distb](https://user-images.githubusercontent.com/14051949/150709223-07234955-68b4-4046-8706-1f84592e5046.png)


Model Architecture: <br/>
Conv1 [Conv (o/p: 512, 48, 48), BatchNorm, ReLU, MaxPool (o/p: 512, 24, 24)] <br/>
Conv2 [Conv (o/p: 128, 24, 24), BatchNorm, ReLU, MaxPool (o/p: 128, 12, 12)] <br/>
Conv3 [Conv (o/p: 64, 12, 12), BatchNorm, ReLU, MaxPool (o/p: 64, 6, 6)] <br/>
Conv4 [Conv (o/p: 64, 6, 6), BatchNorm, ReLU, MaxPool (o/p: 256, 3, 3)] <br/>
Fully Connected Layer (i/p: 256*3*3, o/p: 7) <br/>

Learning Rate: 0.001 <br/>
Optimizer: Adam <br/>
Epochs: 5 <br/>

![accuracy_scores](https://user-images.githubusercontent.com/14051949/150709279-a240e42c-f745-4931-9f40-26591601c91b.png)
