# Activity 2: Exploring Python with Google Colab and AI Assistants

This lab introduces the basics of working with Python in Google Colab. You will practice writing simple Python code, formatting explanations with Markdown, and using an AI assistant to support your work. Complete the tasks in order and keep all of your work in one shared notebook.

#### **1. Getting Started**
1. Open [Google Colab](https://colab.research.google.com).
2. Sign in with your personal Google account **NOT** your Metropolia account.
3. Create a new notebook by selecting **File -> New notebook**.
4. Rename the notebook clearly, for example: **Python Lab - Group 3**.
5. Add the names of all group members in the first text cell so the teacher can identify your work.

<details>
<summary>Sample solution</summary>

Example notebook title:

```text
Group 3 - Session 1 Lab 2
```

Example first text cell:

```markdown
# Python Lab - Group 3

**Group members:**
- Anna 
- Ben 
- Chen
```

</details>

#### **2. Understanding LLMs and AI Assistants**
Before starting the coding tasks, make sure you understand what tool you are using.

1. An **LLM** is a **large language model**. It is an AI system trained on a large amount of text so that it can answer questions, explain ideas, and generate code.
2. An **AI assistant** is the chat tool or interface that you use to interact with the model. In simple terms, the **LLM** is the model behind the system, and the **AI assistant** is the tool you see on the screen.
3. In this lab, you may use an AI assistant powered by an LLM, such as:
   - **Gemini in Colab**: the built-in chat or help tools should be available in your Colab environment,
   - [**Copilot**](https://copilot.microsoft.com), which can also explain concepts and suggest Python code.
4. These tools are useful for getting started, but their answers are not always correct.
5. Always run the code, read it carefully, and test it with your own examples before deciding that it works.

<details>
<summary>Sample solution</summary>

Example summary you could write in your notebook:

```markdown
### What is an LLM?

An LLM is a large language model. It can answer questions and generate code from natural language prompts.
An AI assistant is the tool we use to chat with the model.
In this lab, we can use tools such as Gemini in Colab, Gemini Flash, or Copilot.
We still need to test the generated code ourselves.
```

</details>

#### **3. Python and Markdown Basics**
Before using an AI assistant, complete one very simple exercise to understand the difference between a **code cell** and a **Markdown text cell** in Colab.

1. Insert a **Markdown text cell** and write a short heading and one sentence describing what your notebook is about.
2. Insert a **code cell** and write Python code that:
   - stores your name in a variable,
   - prints a greeting,
   - prints the result of a simple calculation such as `5 + 3`.
3. Run the code cell and make sure the output appears below the cell.

<details>
<summary>Sample solution</summary>

Example text cell:

```markdown
## My First Colab Notebook

This notebook contains simple Python practice tasks.
```

Example code cell:

```python
name = "Sami"
print("Hello,", name)
print("5 + 3 =", 5 + 3)
```

Example output:

```text
Hello, Sami
5 + 3 = 8
```

</details>

#### **4. Warm-Up Exercise**
In this task, you will use an AI assistant such as **Gemini** or [**Copilot**](https://copilot.microsoft.com/) to help you solve a short beginner Python problem.

1. Open a new code cell in your notebook.
2. Decide on one simple Python task you want to solve. Examples:
   - "How do I calculate the sum of numbers in Python?"
   - "Write a Python function to check if a number is even."
3. Open Gemini in Colab, Gemini in your browser, or [Copilot](https://copilot.microsoft.com).
4. Ask the AI assistant for help with your chosen task.
5. Copy the suggested Python code into your Colab notebook.
6. Run the code.
7. Test the code with at least two different inputs and, if needed, improve it.

<details>
<summary>Sample solution</summary>

Example prompt to an AI assistant:

```text
Write a simple Python function that checks whether a number is even.
```

Example code copied into Colab:

```python
def is_even(number):
    return number % 2 == 0

print(is_even(4))
print(is_even(7))
```

Example output:

```text
True
False
```

</details>

#### **5. Exploring Python Tutorials with an AI Assistant**
Now you will explore one beginner Python concept in more detail.

1. Visit this tutorial site: [Python Basics](https://www.pythontutorial.net/python-basics/).
2. Choose one beginner-friendly topic such as **functions**, **loops**, or **lists**.
3. As a group, read the topic introduction and discuss what the concept does.
4. Ask your AI assistant to explain the concept in simple language.
5. Ask your AI assistant to generate a short example program.
6. Copy the example into Colab and run it.
7. Modify the example so it behaves differently. For example:
   - change the values in a list,
   - change the number of loop repetitions,
   - change the function input.
8. Add a short text cell explaining what you changed and what happened.

<details>
<summary>Sample solution</summary>

Example chosen topic: **Loops**

Example prompt to an AI assistant:

```text
Explain Python for loops in a simple way and give me a short example that prints items from a list.
```

Example code cell:

```python
fruits = ["apple", "banana", "orange"]

for fruit in fruits:
    print(fruit)
```

Modified version:

```python
fruits = ["apple", "banana", "orange", "mango"]

for fruit in fruits:
    print("Fruit:", fruit)
```

Example explanation in a text cell:

```markdown
I added `"mango"` to the list and changed the print statement.
Now the loop prints four items and shows the label `Fruit:` before each one.
```

</details>

#### **6. Group Task**
Use what you have learned to build a small Python program together.

1. As a group, choose one small project idea.
2. Possible ideas include:
   - a program that calculates the average of a list of numbers,
   - a multiplication table generator,
   - a number guessing game,
   - a simple quiz with two or three questions.
3. Ask an AI assistant for a first version of the code.
4. Copy the code into Colab and run it.
5. Improve the code together by making it clearer, more correct, or more user-friendly.
6. Test the program carefully.
7. Add a short text cell that explains:
   - what your program does,
   - what changes your group made,
   - what worked well or was difficult.

<details>
<summary>Sample solution</summary>

Example project: **Average calculator**

```python
numbers = [10, 15, 20, 25]
average = sum(numbers) / len(numbers)

print("Numbers:", numbers)
print("Average:", average)
```

Example reflection text cell:

```markdown
### Group Project Reflection

Our program calculates the average of a list of numbers.
We changed the original code by printing the list before the result.
The program worked well after we checked that the list was not empty.
```

</details>

#### **7. Collaboration and Sharing**
1. Use the **Share** button in Google Colab.
2. Give edit or view access to your group members, depending on how you want to work.
3. Check that every group member can open the notebook.
4. Work together in real time to clean up the notebook.
5. Make sure your notebook includes:
   - group member names,
   - completed tasks,
   - code outputs,
   - short explanations in text cells.
6. Save the completed notebook to Google Drive.

<details>
<summary>Sample solution</summary>

Example final checklist:

```markdown
## Final Checklist

- Group members added
- Basic Python and Markdown task completed
- Warm-up task completed
- Python topic explored and modified
- Group task completed
- Notebook shared with group members
```

</details>

#### **Post-Lab Exploration (Optional)**
1. Continue exploring this beginner tutorial: [https://www.pythontutorial.net/python-basics/](https://www.pythontutorial.net/python-basics/).
2. Use an AI assistant to ask follow-up questions if you do not understand a concept.
3. Improve your group task by adding one new feature.
4. Write a short note in your notebook describing what you added.

<details>
<summary>Sample solution</summary>

Example extension idea:

```text
Add input from the user so the program does not use fixed numbers.
```

Example improved code:

```python
numbers_text = input("Enter numbers separated by spaces: ")
numbers = [float(value) for value in numbers_text.split()]
average = sum(numbers) / len(numbers)

print("Average:", average)
```

</details>

