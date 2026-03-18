# Installing and Testing Ollama

#### **Objective**  
By the end of this lab, you will:  
✅ Install **Ollama** on your system.  
✅ Run and test **`phi`** (a small, efficient model for general and coding tasks).  
✅ Run and test **`gemma-2b`** (a  conversational AI model).  
✅ *(Optional)* Install and test **`deepseek-r1`** for advanced coding assistance `ollama run deepseek-r1`.   

---

## **Step 1: Download and Install Ollama**  

### **For Windows & macOS**  
1. Go to **[Ollama's official website](https://ollama.com)**.  
2. Download the installer for your operating system.  
3. Run the installer and follow the on-screen instructions.  

### **For Linux (Ubuntu/Debian)**  
Run the following command in the terminal:  

```sh
curl -fsSL https://ollama.com/install.sh | sh
```

Once installed, restart your terminal.  

---

## **Step 2: Verify Installation**  
To check if Ollama is installed correctly, run:  

```sh
ollama --version
```

If installed, it should return the version number.

---

## **Step 3: Install and Test `phi` (Small Model for General AI & Coding)**  

`phi` is a **lightweight 2.7B model** that works well for both general text-based tasks and simple coding suggestions.  

1. **Download `phi`**:  
   ```sh
   ollama pull phi
   ```
2. **Run `phi` and test it**:  
   ```sh
   ollama run phi 
   ```
3. **Try a coding-related question**:  
   ```sh
   Write a Python function to sort a list of numbers.
   ```
   Observe how the model generates code.

---

## **Step 4: Install and Test `gemma3:1b` (Small Conversational AI)**  

1. **Download `gemma3:1b`**:  
   ```sh
   ollama pull gemma3:1b
   ```
2. **Run `gemma3:1b`**:  
   ```sh
   ollama run gemma3:1b
   ```
3. **Ask a general question**:  
   ```sh
   What is the importance of machine learning?
   ```
--- 
## **Step 5: Install and Test `deepseek-r1:1.5`**  
deepseek-r1:1.5
1. **Download `deepseek-r1:1.5`**:  
   ```sh
   ollama pull deepseek-r1:1.5
   ```
2. **Run `deepseek-r1:1.5`**:  
   ```sh
   ollama run  deepseek-r1:1.5
   ```
3. **Ask a general question**:  
   ```sh
   What is the importance of machine learning?
   ```

---

## **Step 5: Verify Installed Models**  
To check all downloaded models:  
```sh
ollama list
```

To remove a model if needed:  
```sh
ollama rm <model-name>
```

  
<!-- 
docker pull ollama/ollama
docker exec -it b5013af2efb0 ollama run deepseek-r1:1.5b
docker exec -it b5013af2efb0 ollama --version
docker exec -it b5013af2efb0 ollama list
docker exec -it b5013af2efb0 ollama rm <model-name>
-->
