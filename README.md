# Menopause ABM
This is an agent-based model to investigate the evolution of the menopause. Specifically, it allows you to look at the effects of grandmothering and mate choice (both independently and simultaneously) on how the menopause evolves in a population of resident killer whales.

The model was built using [Mesa](https://mesa.readthedocs.io/en/master/), but I edited the batchrunner.py and space.py files.

## Getting started
### Requirements
* Random
* Pandas
* Math
* Copy
* Numpy
* Pathos (this is only needed if you're going to run it multithreaded, but it is included in the requirements.txt anyway)


### Installation
To get started, enter the following in the command line:
``` 
git clone https://gitlab.com/beckypadget/mate-choice-and-menopause.git
```
Then install the requirements using:
```
pip3 install -r requirements.txt
```
Then:
```
cd 'mate-choice-and-menopause'
```
to get into the file.

## Usage
Once you've installed the requirements, you can now edit and run the model. 

To run the model as it is, with graphics, use: 
```python3 run.py``` 
(Mesa doesn't work with Python2). This opens a window in which you can see the whales in space and the sliders on the side allow you to change the parameters of the model and see what happens under different scenarios.

Alternatively, if you want to collect data from the model, you can run it multithreaded using: 
```python3 runbatch.py```
The runbatch file can be edited to suit the number of processes you want to use, as well as the parameters you want to test and the number of iterations and steps. Data is written to file at the end of each iteration.
