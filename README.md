# German Traffic Sign Classification

This project was done as part of my Flatiron School Data Science Bootcamp Module 6 project. In this module, we covered topics such as machine learning, neural networks and natural language processing. My group found a dataset from a Kaggle data science competition consisting of around fifty thousand pictures of German Traffic Signals. 

The recognition of traffic signs is useful utility, because it has applications for self-driving cars. In order to properly navigate streets and highways without human direction, cars must be able to properly recognize traffic signs and properly respond to them. While useful, this was not the purpose of the project for my partners and me. This was our first experience working with neural nets, and it was a learning experience for us. 

The dataset consisted of fifty thousand pictures of German traffic signs divided into forty-three different classes. This dataset differed from most deep learning datasets, which are usually divided into two classes. While most deep learning datasets are divided into a yes/no categorization, our neural network would need to recognize pictures and classify them into forty-three different classes. 

Our initial issue with our neural net was labeling our pictures. While our training dataset of forty thousand photos was properly organized into classes, our testing dataset was not. To solve this issue, we used the attached PDF to manually assign labels to the pictures in our dataset. After proper labeling, we were able to use the Python module Keras to create our neural net.

Our baseline neural net was a convolutional neural net. Convolutional neural nets are the most commonly used neural nets for visual images. While pre-trained neural networks were available for download, we decided to use a simple five-layer neural net consisting of three convolutional layers with pooling followed by two dense layers.

Our first iteration used an RMS Prop optimizer and 5 epochs. Despite only five epochs, we were able to achieve 90% accuracy. While significantly more accurate than random chance, our cost function and accuracy curve indicated that that the error of the neural network had yet to flatten out, indicating that more epochs would need to be run in order to properly train the neural network for our dataset. 

Further iterations of the neural net consisted of twenty epoch runs. We used several different optimizes including an Adam and RMS Prop optimizer. The best accuracy score reached by the neural network was 95.6% accuracy. While the change in optimizer did increase the accuracy, the main contributor to the increased accuracy was the number of epochs run. Our best combination of neural network parameters was an RMS Prop optimizer, rune for twenty epochs. While more epochs could potentially increase the accuracy of our model, we did not view the increase in time to be worth the increase in accuracy. 

When viewing the misclassification errors, we were pleased with the accuracy of our model. While our model was not perfectly accurate in classifying signs, the nature of the errors was promising. While our model was incorrect 4.4% of the time, the model never made errors when it came to the shape and color of the sign. While the sign may “misread” the words on the sign, our neural network could, with 100% accuracy determine the shape and color of a sign. When looking at most frequently misclassified signs, the mislabeled sign pairs were always signs of the same color and shape, but with incorrect “reading” of symbols







### Presentation link  
https://docs.google.com/presentation/d/1k76cQbXxcco-5Ez0Z9QvfXYe8Il5pXxkfVzWobDyuWo/edit#slide=id.g6efed5c069_1_4
