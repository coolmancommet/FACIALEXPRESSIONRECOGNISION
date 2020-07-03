# FACIALEXPRESSIONRECOGNISION :slightly_smiling_face:  	:expressionless: :neutral_face: :pensive: :open_mouth: :frowning_face: :angry: :persevere:

![faceing](https://www.noldus.com/images/content-blog/facereader-authority-element-reliability-performance-emotions-two-rows-illustration.jpg)

This model can be used for prediction of expressions of both still images and real time video. However, in both the cases we have to provide image to the model. In case of real time video the image should be taken at any frame in time and feed it to the model for prediction of expression. The system automatically detects the face using HAAR cascade then its crops it and resize the image to a specific size and give it to the model for prediction. The model will generate seven probability values corresponding to seven expressions. The highest probability value to the corresponding expression will be the predicted expression for that image.

### For runing the project 
#### without gpu version 
first clone the repo:
* `git clone 'https://github.com/coolmancommet/FACIALEXPRESSIONRECOGNISION'`

install the following in your virtual environment :
* `pip install -r install.txt`

this could take some time till then let us know about the files inn this project

* install.txt--therequirements file of the project
* Facial_Expression_Training.ipynb--the main trined model 
* model.json--model architecture we exported from ipynb
* model_weights.h5--weights that we exported from the model 
* model.py--the file which importes the above two files and make a model that will predict the expression in real time 
* haarcascade_frontalface_default.xml--the basic facial locators we use in ipynb

now that you understood the file structure we can run the model to predict the model 
Its time to understand the architecture of the network
![arcchi](https://github.com/coolmancommet/FACIALEXPRESSIONRECOGNISION/blob/master/model.png)

now after activating your virtual environment (if you install the following modules into that ve(recommended))
type in the following command -

* `python main.py`

#### now our project is up and running you should be seeing somthing like this 
![annot](https://github.com/coolmancommet/FACIALEXPRESSIONRECOGNISION/blob/master/.ipynb_checkpoints/Annotation%202020-07-03%20132549.png)

## congratulations you successfully run this project on your machine 
![ronal](https://miro.medium.com/max/1575/1*7plHCvC13Iny6T1QEqlH1w.gif)
