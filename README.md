Here's a guide for installing Jupyter Notebook on Windows:

---

## How to Install Jupyter Notebook on Windows

Jupyter Notebook is an essential tool for data analysis, providing an interactive environment for writing and executing Python code. In this guide, we’ll walk you through the steps to install Jupyter Notebook on a Windows machine.

### **Step 1: Install Python (if not done already)**

Before installing Jupyter, ensure that you have Python installed on your machine. If you haven’t already installed Python, follow the instructions in the previous guide to install the latest version of Python on Windows.

### **Step 2: Install Jupyter Notebook via pip**

1. **Open Command Prompt**:
   - Press `Win + R`, type `cmd`, and press Enter.
   - Alternatively, search for "cmd" in the Windows search bar and hit Enter.

2. **Install Jupyter Notebook**:
   In the Command Prompt, type the following command to install Jupyter using pip (Python's package manager):

```shell
pip install notebook
```
or 

```shell
pip install notebook
```

This will download and install the necessary Jupyter Notebook packages and dependencies.

### **Step 3: Launch Jupyter Notebook**

1. After installation is complete, you can start Jupyter Notebook by typing the following command in Command Prompt:

```shell
jupyter notebook
```

2. The command will launch a local server, and you will see a message in the terminal indicating the URL for the Jupyter Notebook interface, typically something like:

```plaintext
http://localhost:8888/
```

3. Your default web browser will automatically open and display the Jupyter Notebook dashboard. From here, you can create new notebooks, open existing ones, and begin your data analysis projects.

### **Step 4: Create and Test Your First Notebook**

1. On the Jupyter dashboard, click **New** in the top-right corner and select **Python 3**.
2. In the new notebook, type the following code:

```python
print("Welcome to Jupyter Notebook!")
```

3. Press **Shift + Enter** to execute the code. You should see the output below the code cell:

```plaintext
Welcome to Jupyter Notebook!
```

### **Step 5: Closing Jupyter Notebook**

When you're finished, you can close Jupyter Notebook by:
- Clicking **Quit** in the top-right corner of the Jupyter dashboard.
- Alternatively, in Command Prompt, press **Ctrl + C** to stop the server and close the application.

### **Screenshots**

Here are some screenshots of the installation and usage process:

![Jupyter Installation Step 1](jupyter_install_ss1.png)
![Jupyter Installation Step 2](jupyter_install_ss2.png)

### **Conclusion**

You’ve successfully installed and launched Jupyter Notebook on your Windows machine! You can now begin using it for your Python-based data analysis projects. Stay tuned for more tutorials on how to make the most of Jupyter Notebook for your data analysis workflow.

---

This guide provides the step-by-step instructions for installing and using Jupyter Notebook on Windows. Let me know if you need any additional information!
