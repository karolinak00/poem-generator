# Dataset
In the project dataset from https://www.kaggle.com/datasets/ultrajack/modern-renaissance-poetry was used. 

# About project
Project consists of two recurrent neural networks: the stateful and stateless one. Firstly, a stateful model was trained because it can find patterns in the data and learns faster than stateless model. Then, weights from stateful model were copied to the stateless model, so user doesn't need to give on the input data with fixed size like it's expected in stateful model.

# How to run the model?
To run this code, open *poem_generator.ipynb* file in Jupyter Notebook. If you are using desktop application (for example Anaconda), download *stateless_model.h5* file. If you are using Jupyter Notebook in cloud (for example Google Colab), upload this file to your workspace. Then, change the paths in *Constants* section. 

Run code in all cells in following sections:
- Imports
- Constants
- Loading the model
- Generating the poem

To generate the poem, go to the end of the notebook. There is a cell with following code:

##poem = generate_poem(stateless_model, start_string='You ', len=500)
##print(poem)

Here you can modify parameter *start_string* (which is beginning of the sequence that will be generated) and *len* which is length of the sequence. If you have your own model, you can replace *stateless_model* with your own model. Have fun with generating the poems :)
