# Homework #2: Music Tagging with Deep Learning 
Music tagging is an important task that can be used in many musical applications such as music search or recommender systems. The goals of homework part 2 are follows: 

* Experiencing the whole pipeline of deep learning based system: data preparation, feature extraction, model training and evaluation
* Getting familiar with various CNN models for music classification 
* Using Pytorch in practice


### Preparing The Dataset
We use the [magnatagatune](https://mirg.city.ac.uk/codeapps/the-magnatagatune-dataset) dataset which has been the most widely used in the music tagging task.  The MagnaTagATune dataset consists of 25k music clips from 6,622 unique songs. The dataset contains 30-second audio files including 189 different tags. For this assignment, we will use a subset consisting of 9074 samples with 8 seconds of audio and only 50 genres.


### Baseline: Training an 1D CNN model from Scratch
The Python notebook file for the baseline algorithm ([GCT634-HW2.ipynb](https://colab.research.google.com/drive/1JJyPBZ4lg9y4lCQNLol28_L6GqY6lEAI?usp=sharing))
is provided so that you can easily start the homework and also compare with your own algorithm. The baseline model extracts mel-spectrogram and has a simple set of 1D CNN model that includes 1D convolutional layers, batch normalization, max-pooling and fully-connected layer.


### Question 1: Implement a 2D CNN model 
The model configuraiton and startup code are given in the Jupyter Notebook file. You can complete it by filling in the "to-do" area.

### Question 2: Improve the performenace
Now it is your turn. You can improve the model performance with your own idea. There are many ways to improve it. The followings are possible ideas: 

* You can try different optimizers or learning rate on the 1D or 2D CNN model above.

* You can build a different configuration of CNN models, referring to existing CNN models (https://github.com/minzwon/sota-music-tagging-models). We recommend you to reproduce "Short-Chunk CNN" which is known to be simple but effective.

* You can optionally augment data using digital audio effects. For more detail, see this tutorial (https://music-classification.github.io/tutorial/part3_supervised/data-augmentation.html)


## Deliverables
You should submit your Python Notebook (.ipynb) and homework report (.pdf file) to KLMS. The report should include:
* Algorithm Description
* Experiments and Results
* Discussion

## Evaluation Criteria
* Did you analyze the dataset and labels and write a suitable hypothesis?
* Did you construct a deep learning model and write down the difference from the baseline?
* Did you write findings and discussions?
* English does not need to be flawless but the text should be understandable and the code should be re-implementable.

