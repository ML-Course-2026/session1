# Optional Activity: Installing and Testing Ollama

#### **Objective**
By the end of this optional activity, you should be able to:
- install **Ollama** on your computer,
- verify that Ollama works from the command line,
- download and run at least one model locally,
- test the model with a simple prompt,
- understand that Ollama can be used in both terminal and GUI-based chat interfaces.

This activity is about getting started with **local AI models**. You do **not** need to test every possible model.

---

## **What Is Ollama?**

**Ollama** is a tool for running AI models locally on your own computer.

You can use Ollama in two common ways:
- **Command line**, for example with `ollama run model-name`
- **GUI applications**, which provide a chat interface similar to ChatGPT

In other words, Ollama does not have to be used only in a terminal. It can also be connected to graphical interfaces that feel like a normal chat application. 

Ollama is only one way to use AI models. In this activity, Ollama is used for **local models**. More broadly, there are also:
- **local models** running on your own computer,
- **cloud models** running on remote servers,
- different model families for different tasks and hardware sizes.

The examples in this activity are only a small sample.

---

## **Step 1: Download and Install Ollama**

### **For Windows and macOS**
1. Go to [Ollama's official website](https://ollama.com).
2. Download the installer for your operating system.
3. Run the installer and follow the instructions.

### **For Linux (Ubuntu/Debian)**
Run the following command in the terminal:

```sh
curl -fsSL https://ollama.com/install.sh | sh
```

After installation, restart the terminal.

---

## **Step 2: Verify the Installation**

To check that Ollama is installed correctly, run:

```sh
ollama --version
```

If the installation worked, Ollama will print a version number.

---

## **Step 3: Run Your First Model**

Start with one small model so that the download is manageable.

Example:

```sh
ollama pull phi
ollama run phi
```

When the model starts, try a simple prompt such as:

```text
Write a Python function to sort a list of numbers.
```

Observe the response and note whether the model produces code, explanation, or both.

---

## **Step 4: Try Another Model**

You can test a different model and compare the answers.

For example:

```sh
ollama pull gemma3:1b
ollama run gemma3:1b
```

Try a general prompt such as:

```text
What is the importance of machine learning?
```

If your computer has enough memory and storage, you may also try other models.

---

## **Step 5: Optional Additional Models**

If you want to explore more, you can try additional models from the Ollama library.

Examples include:
- [Gemma 3](https://ollama.com/library/gemma3)
- [Qwen 3](https://ollama.com/library/qwen3)
- [Qwen 3.5](https://ollama.com/library/qwen3.5)

You may also try [models](https://ollama.com/search) such as `deepseek-r1`, depending on your computer and the model size you choose.

Example:

```sh
ollama pull deepseek-r1:1.5b
ollama run deepseek-r1:1.5b
```

Important note:
- larger models usually require more RAM,
- some models run well on lightweight laptops,
- others may be too large or too slow for your machine.

---

## **Step 6: Using Ollama with a GUI**

Ollama can also be used with a **graphical chat interface** instead of only the terminal.

This means you can use local models in a GUI that feels similar to ChatGPT, where you:
- type prompts into a chat window,
- read replies in a conversation view,
- switch between models more easily.

In practice, this can be more comfortable for beginners than typing everything in the terminal. 

---

## **Step 7: Check Installed Models**

To view all downloaded models, run:

```sh
ollama list
```

To remove a model you no longer need, run:

```sh
ollama rm <model-name>
```

---

## **What You Should Learn from This Activity**

After this activity, you should understand that:
- Ollama lets you run some AI models locally,
- models can be used from the terminal or from a GUI,
- different models have different sizes and strengths,
- the examples in this activity are only a starting point,
- many other models exist, including both local and cloud-based options.


<!-- 
docker pull ollama/ollama
docker exec -it b5013af2efb0 ollama run deepseek-r1:1.5b
docker exec -it b5013af2efb0 ollama --version
docker exec -it b5013af2efb0 ollama list
docker exec -it b5013af2efb0 ollama rm <model-name>
-->
