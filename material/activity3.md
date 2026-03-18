# activity 3

> In part 2 and part 3, the goal **is not to understand the code itself**. Instead, it's an opportunity to `experiment with Google Colab` and become familiar with `using code cells exclusively`.

### Part 1/3: Using Google Colab with Basic Python

**Step 1: Accessing Google Colab**
- Open your web browser and navigate to [Google Colab](https://colab.research.google.com/).
- Sign in with your Google account. If you don't have one, you'll need to create one.

**Step 2: Creating a New Notebook**
- Click on the "New Notebook" button to create a new Colab notebook.

**Step 3: Writing Basic Python Code**
- In the first cell of your notebook, type the following code to print "Hello, world!":

```python
print("Hello, world!")
```

- To execute the code in the cell, either press Shift + Enter or click on the "Play" button located on the left side of the cell.

**Step 4: Importing Libraries**
- Importing libraries allows you to extend the functionality of Python. Let's import the pandas library as an example:

```python
import pandas as pd
```

**Step 5: Loading Data with Pandas**
- You can use pandas to load data from various sources. For example, let's load a CSV file named "iris.data" from a URL:

```python
url = 'https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data'
df = pd.read_csv(url)
```

-
**Step 6: Exploring Data**
- Once the data is loaded, you can explore it using pandas functions. For example, you can display the first few rows of the DataFrame:

```python
df.head()
```

**Step 7: Analyzing Data**
- You can perform various data analysis tasks using pandas. For example, you can calculate summary statistics:

```python
summary_stats = df.describe()
print(summary_stats)
```

**Step 8: Saving Your Work**
- To save your work, go to File > Save or File > Save a Copy in Drive. This will save your notebook to your Google Drive.

**Step 9: Sharing Your Notebook**
- You can share your notebook with others by clicking on the Share button in the top-right corner of the Colab interface. You can either share it directly with specific people or generate a shareable link.

**Step 10: Exiting Google Colab**
- Once you've finished your work, you can close the Colab notebook tab in your browser. Your work will be automatically saved in your Google Drive.

### Part 2/3: Visualization

> In this part, the goal **is not to understand the code itself**. Instead, it's an opportunity to `experiment with Google Colab` and become familiar with `using code cells exclusively`.

To visualize the Iris dataset, you can use various plotting libraries in Python, such as Matplotlib, Seaborn, or Plotly. Here's an example using Matplotlib and Seaborn to create some basic visualizations:

First, let's import the required libraries and load the Iris dataset:

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load the Iris dataset
url = 'https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data'
column_names = ['sepal_length', 'sepal_width', 'petal_length', 'petal_width', 'species']
iris = pd.read_csv(url, header=None, names=column_names)
```

Now, let's create some basic visualizations:

1. **Pairplot**: This plot shows pairwise relationships between variables along with the distribution of each variable.

```python
sns.pairplot(iris, hue='species')
plt.show()
```

2. **Boxplot**: This plot shows the distribution of a continuous variable (e.g., sepal length) for different categories (e.g., species).

```python
plt.figure(figsize=(10, 6))
sns.boxplot(data=iris, x='species', y='sepal_length')
plt.title('Sepal Length Distribution by Species')
plt.show()
```

3. **Histogram**: This plot shows the distribution of a single variable (e.g., sepal length).

```python
plt.figure(figsize=(8, 6))
sns.histplot(data=iris, x='petal_width', kde=True)
plt.title('Petal Width Distribution')
plt.xlabel('Petal Width')
plt.ylabel('Frequency')
plt.show()
```

### Part 3/3: Using MNIST Dataset in Google Colab

> In this part, the goal **is not to understand the code itself**. Instead, it's an opportunity to `experiment with Google Colab` and become familiar with `using code cells exclusively`.


**Step 1: Accessing Google Colab**
- Open your web browser and navigate to [Google Colab](https://colab.research.google.com/).
- Sign in with your Google account. If you don't have one, you'll need to create one.

**Step 2: Creating a New Notebook**
- Click on the "New Notebook" button to create a new Colab notebook.

**Step 3: Loading the MNIST Dataset**
- In the first cell of your notebook, install the TensorFlow library, which includes the MNIST dataset:

```python
!pip install tensorflow
```

- Next, import the TensorFlow library and load the MNIST dataset:

```python
import tensorflow as tf
mnist = tf.keras.datasets.mnist
(x_train, y_train), (x_test, y_test) = mnist.load_data()
```

**Step 4: Exploring the Dataset**
- You can explore the loaded dataset to understand its structure and contents. For example, you can display the shape of the training and test data:

```python
print('Training data shape:', x_train.shape)
print('Training labels shape:', y_train.shape)
print('Test data shape:', x_test.shape)
print('Test labels shape:', y_test.shape)
```

**Step 5: Preprocessing the Data (Optional)**
- Depending on your analysis goals, you may need to preprocess the data. For example, you can normalize the pixel values to the range [0, 1]:

```python
x_train, x_test = x_train / 255.0, x_test / 255.0
```

**Step 6: Building a Simple Model (Optional)**
- You can build a simple neural network model to classify the MNIST digits. Here's an example of a basic model using TensorFlow's Keras API:

```python
model = tf.keras.models.Sequential([
    tf.keras.layers.Flatten(input_shape=(28, 28)),
    tf.keras.layers.Dense(128, activation='relu'),
    tf.keras.layers.Dropout(0.2),
    tf.keras.layers.Dense(10)
])

model.compile(optimizer='adam',
              loss=tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True),
              metrics=['accuracy'])

model.summary()
```

**Step 7: Training the Model (Optional)**
- You can train the model using the training data and evaluate its performance on the test data:

```python
model.fit(x_train, y_train, epochs=5)
test_loss, test_acc = model.evaluate(x_test, y_test, verbose=2)
print('\nTest accuracy:', test_acc)
```

**Step 8: Saving Your Work**
- To save your work, go to File > Save or File > Save a Copy in Drive. This will save your notebook to your Google Drive.

**Step 9: Visualization**

To visualize the images in the MNIST dataset, you can use Matplotlib, which is a popular plotting library in Python. Here's how you can visualize MNIST images in Google Colab:

```python
import matplotlib.pyplot as plt

# Plot the first few images from the MNIST dataset
plt.figure(figsize=(10, 10))
for i in range(25):
    plt.subplot(5, 5, i + 1)
    plt.imshow(x_train[i], cmap='gray')
    plt.axis('off')
    plt.title(f'Label: {y_train[i]}')
plt.show()
```

In this code:

- We import Matplotlib as `plt`.
- We create a new figure with a size of 10x10 inches using `plt.figure(figsize=(10, 10))`.
- We loop through the first 25 images in the training dataset.
- For each image, we plot it using `plt.imshow()` with a grayscale colormap (`cmap='gray'`).
- We turn off the axes using `plt.axis('off')` to remove the axis ticks and labels.
- We set the title of each subplot to the corresponding label using `plt.title()`.

You can adjust the number of images to display by changing the range in the loop. This code will display a 5x5 grid of images with their corresponding labels.




