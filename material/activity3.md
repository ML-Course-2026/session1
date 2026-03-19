# Activity 3: More Practice with Google Colab

This optional activity is for practicing how to use Google Colab.

The main goal is to become comfortable with:
- opening a notebook,
- adding text cells and code cells,
- running code cells,
- copying code into cells,
- viewing outputs,
- saving and sharing your work.

### Part 1 of 2: First Steps in Google Colab

In this part, you will practice the most basic Colab actions. The goal is to learn how to open a notebook, add cells, run a small piece of Python code, and save your work.

1. Open [Google Colab](https://colab.research.google.com/).
2. Sign in with your **Personal** Google account.
3. Create a new notebook.
4. Rename the notebook so it has a clear name, for example: **Activity 3 - Colab Practice**.
5. Add a **text cell** at the top of the notebook and type a short title, such as **My Colab Practice Notebook**.
6. Add one **code cell** below the text cell.
7. In the code cell, type and run the following code:

```python
print("Hello, world!")
```

8. Run the cell by pressing **Shift + Enter** or by clicking the **Run** button.
9. Confirm that the output appears below the cell.
10. Save your notebook to Google Drive.
11. If you are working with others, use the **Share** button to share the notebook.

### Part 2 of 2: Markdown Basics in Colab

In this part, you will practice using **Markdown text cells** in Colab. You do not need much Python here. The main goal is to learn how to format text so your notebook is easier to read.

Colab has two main cell types:
- **Code cells** for Python code
- **Text cells** for Markdown

To edit Markdown in Colab, insert a text cell and double-click it to see the Markdown source.

1. Add a new **text cell**.
2. Copy the example below into the text cell.
3. Run the text cell so you can see the formatted result.
4. After that, modify the text with your own group name, course name, or short notes.

Use this example, adapted from the Colab Markdown guide and basic Markdown syntax examples:

```markdown
# My Colab Markdown Practice

## About This Notebook

This notebook is for practicing **Markdown** in Google Colab.

We can make text *italic*, **bold**, or `monospace`.

### A Short List

- Open Colab
- Add a text cell
- Add a code cell

### A Numbered List

1. Write Markdown
2. Run the text cell
3. Check the formatted output

### A Link

Visit [Google Colab](https://colab.research.google.com/).

### A Quote

> Markdown helps make notebooks easier to read.

---
```

5. Add another **text cell** and create a small table like this:

```markdown
| Item | Meaning |
|---|---|
| Text cell | Used for Markdown |
| Code cell | Used for Python |
```

6. Run the table cell and check that the table appears correctly.
7. Add one final **code cell** with only a very small amount of Python:

```python
print("Markdown and Python can be used in the same Colab notebook.")
```

8. Run the code cell.
9. Save your notebook.

### What You Should Learn from This Activity

After this activity, you should be able to:
- open Google Colab and create a notebook,
- add both text cells and code cells,
- write simple Markdown in a text cell,
- run a small Python code cell,
- save and share your notebook.

You do **not** need to understand advanced Python in this activity. The focus is on using Colab and formatting notebook content clearly.

### Markdown Reference Used in This Lab

Below is a short explanation of the Markdown elements used in this activity.

#### 1. Headings
Headings create titles and section titles in a text cell.

Example:

```markdown
# Main Title
## Section Title
### Smaller Section Title
```

- `#` creates a large heading.
- `##` creates a smaller heading.
- `###` creates an even smaller heading.

#### 2. Bold Text
Bold text highlights important words.

Example:

```markdown
This is **bold** text.
```

#### 3. Italic Text
Italic text is useful for light emphasis.

Example:

```markdown
This is *italic* text.
```

#### 4. Monospace or Inline Code
Use backticks for code words, commands, or short code fragments.

Example:

```markdown
Use `print()` in a Python code cell.
```

#### 5. Unordered Lists
Unordered lists are bullet-point lists.

Example:

```markdown
- First item
- Second item
- Third item
```

#### 6. Ordered Lists
Ordered lists are numbered lists.

Example:

```markdown
1. First step
2. Second step
3. Third step
```

#### 7. Links
Links let you connect to websites.

Example:

```markdown
[Google Colab](https://colab.research.google.com/)
```

#### 8. Blockquotes
Blockquotes are useful for notes, quotes, or highlighted comments.

Example:

```markdown
> This is a quoted note.
```

#### 9. Horizontal Rule
A horizontal rule creates a visual divider between sections.

Example:

```markdown
---
```

#### 10. Tables
Tables organize information into rows and columns.

Example:

```markdown
| Item | Meaning |
|---|---|
| Text cell | Used for Markdown |
| Code cell | Used for Python |
```

### Final Note

In Google Colab, Markdown is used in **text cells** and Python is used in **code cells**.
If you forget the syntax, you can return to this section and copy the examples.





<!-- 


In Parts 2 and 3, the goal is **not** to fully understand the code. You are using the code as a way to practice the Colab workflow. 

### Part 2 of 3: Creating Simple Visualizations in Colab

In this part, the goal is **not** to understand every line of code. The goal is to practice copying code into Colab, running cells, and viewing outputs.

1. Open a new Colab notebook, or continue in the same notebook if your teacher allows it.
2. Copy the following code into a code cell and run it:

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

url = "https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data"
column_names = ["sepal_length", "sepal_width", "petal_length", "petal_width", "species"]
iris = pd.read_csv(url, header=None, names=column_names)
```

3. Add a new code cell and run this pairplot example:

```python
sns.pairplot(iris, hue="species")
plt.show()
```

4. Add a new code cell and run this boxplot example:

```python
plt.figure(figsize=(10, 6))
sns.boxplot(data=iris, x="species", y="sepal_length")
plt.title("Sepal Length Distribution by Species")
plt.show()
```

5. Add a new code cell and run this histogram example:

```python
plt.figure(figsize=(8, 6))
sns.histplot(data=iris, x="petal_width", kde=True)
plt.title("Petal Width Distribution")
plt.xlabel("Petal Width")
plt.ylabel("Frequency")
plt.show()
```

6. Look at the outputs and confirm that each chart appears below its cell.
7. Save your notebook.

### Part 3 of 3: Running an MNIST Example in Colab

In this part, the goal is again **not** to fully understand the code. The goal is to practice running a longer Colab workflow and seeing different types of output.

1. Open a new Colab notebook, or continue in the same notebook if your teacher allows it.
2. In a code cell, run the following command:

```python
!pip install tensorflow
```

3. In a new code cell, copy and run the following code to load the MNIST dataset:

```python
import tensorflow as tf

mnist = tf.keras.datasets.mnist
(x_train, y_train), (x_test, y_test) = mnist.load_data()
```

4. In a new code cell, run the following to inspect the dataset:

```python
print("Training data shape:", x_train.shape)
print("Training labels shape:", y_train.shape)
print("Test data shape:", x_test.shape)
print("Test labels shape:", y_test.shape)
```

5. If you want, run this optional preprocessing step:

```python
x_train, x_test = x_train / 255.0, x_test / 255.0
```

6. If you want, run this optional model-building example:

```python
model = tf.keras.models.Sequential([
    tf.keras.layers.Flatten(input_shape=(28, 28)),
    tf.keras.layers.Dense(128, activation="relu"),
    tf.keras.layers.Dropout(0.2),
    tf.keras.layers.Dense(10)
])

model.compile(
    optimizer="adam",
    loss=tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True),
    metrics=["accuracy"]
)

model.summary()
```

7. If you want, run this optional training example:

```python
model.fit(x_train, y_train, epochs=5)
test_loss, test_acc = model.evaluate(x_test, y_test, verbose=2)
print("\nTest accuracy:", test_acc)
```

8. To view sample images from the dataset, run this code in a new cell:

```python
import matplotlib.pyplot as plt

plt.figure(figsize=(10, 10))
for i in range(25):
    plt.subplot(5, 5, i + 1)
    plt.imshow(x_train[i], cmap="gray")
    plt.axis("off")
    plt.title(f"Label: {y_train[i]}")
plt.show()
```

9. Confirm that a grid of handwritten digit images appears below the cell.
10. Save your notebook to Google Drive.

### What You Should Learn from This Activity

After this activity, you should be able to:
- open Google Colab and create a notebook,
- add and run code cells,
- copy code into cells and execute it,
- view tables, text output, and charts,
- save and share your notebook.

You do **not** need to fully understand all of the code in Parts 2 and 3.
-->
