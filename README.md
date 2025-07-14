# Matplotlib and pyplot
Complete the tasks in the Python Notebook in this repository. To be submitted for credit, all changes must be committed and pushed to this repository (do not create your own repository unless instructed to on the course website).

## Rubric
Each question is worth two points:
* Data plotted as described by the question (1 pt)
* Plot contains required elements (title, axis labels, axis titles, legend if required)

## Objective
This exercise is used to reinforce key Python visualization skills. It offers practice with web-enabled Jupyter notebooks and lays some important foundations for presenting information obtained from mining the web and processing language. The Matplotlib library includes the pyplot module which provides a simple interface for building charts.

### Step 1: Copy the base repository to local machine
* `git clone` [pyplot.ipynb](https://github.com/wmnlp-materials/pyplot/blob/master/pyplot.ipynb)

### Step 2: Set Up and Activate Virtual Environment
* `python -m venv .venv`
* `.venv/Scripts/activate`

### Create .gitignore and Install Packages
* Create .gitignore.
* Create requirements.txt to install packages.
* `pip install -r requirements.txt`

### Open Notebook and Complete Tasks
* Make sure kernal is selected.
* Add a viewable, clickable link to GitHub repo after name in the Markdown Introduction.
* Use Markdown headings to show content by each question number.
* Complete the questions.
    - `from collections import Counter`
    - `from random import randint`
    - `import matplotlib.pyplot as plt`
    - `import random`
    - Create charts using `plt.bar`, `plt.plot`, and `plt.scatter`

### Execute the notebook

### Commit and push to GitHub
* `git add .`
* `git commit -m "Meaningful comment"`
* `git push`
* Verify the notebook appears correctly in GitHub.

### Export to HTML and Finalize Repo
* `!jupyter nbconvert --to html pyplot.ipynb`

