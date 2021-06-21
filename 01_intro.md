# Lesson 1: Intro

Link: [Lesson 1: Intro](https://github.com/Jeff-Adler/fastbook/blob/master/01_intro.ipynb)

## Definitions

We just covered a lot of information so let's recap briefly, <> provides a handy vocabulary.

[[dljargon]]
.Deep learning vocabulary
[options="header"]
|=====
| Term | Meaning
|Label | The data that we're trying to predict, such as "dog" or "cat"
|Architecture | The _template_ of the model that we're trying to fit; the actual mathematical function that we're passing the input data and parameters to
|Model | The combination of the architecture with a particular set of parameters
|Parameters | The values in the model that change what task it can do, and are updated through model training
|Fit | Update the parameters of the model such that the predictions of the model using the input data match the target labels
|Train | A synonym for _fit_
|Pretrained model | A model that has already been trained, generally using a large dataset, and will be fine-tuned
|Fine-tune | Update a pretrained model for a different task
|Epoch | One complete pass through the input data
|Loss | A measure of how good the model is, chosen to drive training via SGD
|Metric | A measurement of how good the model is, using the validation set, chosen for human consumption
|Validation set | A set of data held out from training, used only for measuring how good the model is
|Training set | The data used for fitting the model; does not include any data from the validation set
|Overfitting | Training a model in such a way that it _remembers_ specific features of the input data, rather than generalizing well to data not seen during training
|CNN | Convolutional neural network; a type of neural network that works particularly well for computer vision tasks
|=====

What makes deep learning distinctive is a particular class of architectures: the architectures based on neural networks. 

Creating a model that can recognize the content of every individual pixel in an image is called segmentation
- Like phonology!!

Training set vs Validation set vs Test set

## Tips

Choose Run All Above from the Cell menu to run all cells above the point where you are

To put it bluntly, if you're a senior decision maker in your organization (or you're advising senior decision makers), the most important takeaway is this: if you ensure that you really understand what test and validation sets are and why they're important, then you'll avoid the single biggest source of failures we've seen when organizations decide to use AI. For instance, if you're considering bringing in an external vendor or service, make sure that you hold out some test data that the vendor never gets to see. Then you check their model on your test data, using a metric that you choose based on what actually matters to you in practice, and you decide what level of performance is adequate. (It's also a good idea for you to try out some simple baseline yourself, so you know what a really simple model can achieve. Often it'll turn out that your simple model performs just as well as one produced by an external "expert"!)

## Questionnaire

Do you need these for deep learning?

Lots of math T / F
Lots of data T / F
Lots of expensive computers T / F
A PhD T / F
Name five areas where deep learning is now the best in the world.

What was the name of the first device that was based on the principle of the artificial neuron?
Based on the book of the same name, what are the requirements for parallel distributed processing (PDP)?
What were the two theoretical misunderstandings that held back the field of neural networks?
What is a GPU?
Open a notebook and execute a cell containing: 1+1. What happens?
Follow through each cell of the stripped version of the notebook for this chapter. Before executing each cell, guess what will happen.
Complete the Jupyter Notebook online appendix.
Why is it hard to use a traditional computer program to recognize images in a photo?
What did Samuel mean by "weight assignment"?
What term do we normally use in deep learning for what Samuel called "weights"?
Draw a picture that summarizes Samuel's view of a machine learning model.
Why is it hard to understand why a deep learning model makes a particular prediction?
What is the name of the theorem that shows that a neural network can solve any mathematical problem to any level of accuracy?
What do you need in order to train a model?
How could a feedback loop impact the rollout of a predictive policing model?
Do we always have to use 224×224-pixel images with the cat recognition model?
What is the difference between classification and regression?
What is a validation set? What is a test set? Why do we need them?
What will fastai do if you don't provide a validation set?
Why is a GPU useful for deep learning? How is a CPU different, and why is it less effective for deep learning?
Try to think of three areas where feedback loops might impact the use of machine learning. See if you can find documented examples of that happening in practice.