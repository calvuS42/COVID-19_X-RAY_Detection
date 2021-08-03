# COVID-19_X-RAY_Detection

The goal of the project was to create a model that could effectively distinguish between Covid patients and healthy people. Since this task was performed in May 2020, high-quality datasets did not exist at that time. In order to create a large enough sample for training, I had to combine several separate datasets (module create_dataset), which resulted in a third class - "pneumonia patients".

A separate task was to show exploratory analysis skills, which was implemented in the "describe" module. 

The model used in the project consisted of a pre-trained on ImageNet ResNet50 and a head which was further trained on the created dataset. The main mistake and failure of this project was imbalance in the amount of data of each class, so that the model with wrong conclusions (that the person is healthy) still scored 80%+ accuracy on the test data. 
