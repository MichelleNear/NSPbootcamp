# Installation and package management

We have installed Anaconda. This is a package management system, which helps us [install packages and create and maintain separate environments](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#) for separate programming tasks. One of the great things about python is that we can leverage all of that public and free code out there. Great! One disadvantage: not everyone in the world has coordinated their code bases to work with everyone else's 🤼‍♂️ 🤺 🖥. (ha!) this means that Jane's very_useful_package may require a numpy version that conflicts with Bob's pretty_good_tool. The solution: create seprate environments for working with Jane's very_useful_package and Bob's pretty_good_tool. For science, examples include separate environemnts for image analysis, Arduino control, a course, and a home project for scraping data from twitter. 

### Confirm you have created an Anaconda environment called NSPbootcamp
#### run the following line:
<br>```conda activate NSPbootcamp```
#### success?
<br>

### Add all of the needed packages to NSPbootcamp
#### There are a few different ways to add pacakges to your environment. In an Anaconda environment, choice A is to use: ```conda install name_of_my_package```. This depends on the package having an Anaconda channel. lot's of packages do. but some don't, in which case they almost certainly have a PyPi channel, in which case you need to use ```pip install name_of_my_package```. In order to use ```pip```, let's make sure our Anaconda environment has ```pip```:
<br> ```conda install pip```

#### here's another key element of how we'll use python: Jupyter Lab, for Jupyter ipython notebooks. let's install it: 
<br> ```conda install jupyterlab```

#### we could keep going like this, one at a time. but we can also do a bunch at once (note we could have also done this when we created the environment, but we are learning here!)
<br> ```conda install scipy seaborn scikit-image fsspec```

### finally, let's do a pip line to install a couple of things that aren't on Anaconda: 
<br> ```pip gcsfs scanpy[louvain] allensdk==2.0.0```
<br>

### We should be good for the next couple of days. 
Of course, we can always add packages later as we need them, using a terminal and ```conda install name_of_my_package```or ```pip install name_of_my_package```
