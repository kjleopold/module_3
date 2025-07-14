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
* Add a viewable, clickable link to GitHub repo after name in the Markdown Introduction.
* Use Markdown headings to show content by each question number.
* Complete the questions.
    - `from collections import Counter`
    - `from random import randint`
    - `import matplotlib.pyplot as plt`
    - `import random`
    - Create charts
```
# make a bar plot with an appropriate title, correct xtick labels, and labeled axes

sort_letters = sorted(letter_freq.keys())
sort_counts = [letter_freq[char] for char in sort_letters]

plt.figure(figsize=(12, 6))
bars = plt.bar(sort_letters, sort_counts, color='orchid', edgecolor='black')

plt.title("Letter Frequency in Passage")
plt.xlabel("Letters")
plt.ylabel("Frequency")
plt.xticks(sort_letters)

# Add labels on top of each bar
for bar in bars:
    height = bar.get_height()
    plt.text(bar.get_x() + bar.get_width() / 2, height + 1, str(height), ha='center', va='bottom', fontsize=8)

plt.tight_layout()
plt.show()
```

```
# Line plot
ax1.plot(x, random_numbers, marker='p', markersize=10, markerfacecolor='purple', color='skyblue')
ax1.set_title("Line Plot")
ax1.set_xlabel("Index")
ax1.set_ylabel("Random Number")

# Scatter plot
ax2.scatter(x, random_numbers, marker='*', s=100, color='magenta')
ax2.set_title("Scatter Plot")
ax2.set_xlabel("Index")
ax2.set_ylabel("Random Number")

plt.tight_layout()
plt.show()
```

```
# Plot both datasets on the same axes
plt.figure(figsize=(10, 5))

plt.plot(sizes, insertion_sort_times, marker='o', color='teal', label='Insertion Sort')
plt.plot(sizes, merge_sort_times, marker='s', color='purple', label='Merge Sort')

plt.title("Sorting Time vs List Size")
plt.xlabel("List Size")
plt.ylabel("Time (seconds)")
plt.legend()
plt.grid(True)
plt.tight_layout()

plt.show()
```


### Execute the notebook

### Commit and push to GitHub
* `git add .`
* `git commit -m "Meaningful comment"`
* `git push`
* Verify the notebook appears correctly in GitHub.

### Export to HTML and Finalize Repo
* `!jupyter nbconvert --to html pyplot.ipynb`

