# bird_classification

The project involves the classification of bird species using pre-trained visual models. The dataset used for this task is the Kaggle Bird Species dataset. Two popular pre-trained visual models, ResNet50V2 and InceptionResNetV2, were used and trained with transfer learning and fine-tuned with ImageNet weights. During experimentation, hyperparameters were varied including training epochs, optimizer learning rate, etc.

The models were trained by freezing the convolutional layers and first training just the dense (fully connected) layers with varying hyperparameters known as "transfer learning". Following transfer learning, the whole model was set to be trainable and was further trained with very low learning rate, known as fine-tuning. The hyperparameters were varied to find the best performing model.

The ResNet50V2 model performed well in all configurations with a classification accuracy of over 95% in all cases. The best performing model was ResNet50V2 trained with the Adam optimizer with a static learning rate of 0.0002 during transfer learning and a learning rate of 0.000002 during fine-tuning. The best performing classification model with an accuracy score of 0.984 was observed. With the best results observed from the above hyperparameters, InceptionResNetV2 was used with similar hyperparameters, and similar performance was recorded.

Overall, the project involved using pre-trained visual models to classify bird species from the Kaggle Bird Species dataset. Various hyperparameters were tuned to find the best performing model, and the ResNet50V2 model with the Adam optimizer and specific learning rates was found to perform the best.
