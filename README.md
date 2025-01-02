# Installing Jupyter Notebook or Anaconda on Windows

For the easiest and most trouble-free experience, it is highly recommended to install **Anaconda** or **Miniconda**. These distributions come with Jupyter Notebook pre-installed along with additional tools, minimizing potential issues during installation. However, if you prefer a lightweight approach, standalone Jupyter Notebook installation instructions are also provided.

---

## Prerequisites

- **Python Installed**: Ensure Python is installed if you plan to use Jupyter directly. Otherwise, installing Anaconda or Miniconda includes Python automatically.
- **Operating System**: Windows 10 or later.

---

## Recommended: Install Anaconda or Miniconda

### Why Choose Anaconda or Miniconda?

| Feature                     | Anaconda                                                               | Miniconda                                                             |
|-----------------------------|------------------------------------------------------------------------|----------------------------------------------------------------------|
| **Includes conda**           | Yes                                                                   | Yes                                                                  |
| **Includes Anaconda Navigator** | Yes                                                                   | No                                                                   |
| **Number of Packages**       | Over 300                                                              | Less than 70                                                         |
| **Install Space Required**   | Approximately 4.4 GB                                                  | Approximately 480 MB                                                 |

- **Anaconda**: Best for beginners and those who want a fully equipped environment with pre-installed libraries and tools.
- **Miniconda**: A lightweight option for advanced users who prefer to install only the necessary libraries.

### Installation Steps:

1. **Download the Installer**:
   - [Download Anaconda](https://www.anaconda.com/products/distribution)
   - [Download Miniconda](https://docs.conda.io/en/latest/miniconda.html)

2. **Run the Installer**:
   - Double-click the installer and follow the on-screen instructions.
   - During installation:
     - **Add Anaconda to my PATH environment variable**: Not recommended.
     - **Register Anaconda as my default Python**: Recommended.

3. **Launch Jupyter Notebook**:
   - Open the **Anaconda Navigator** and launch Jupyter Notebook.
   - Alternatively, open Command Prompt and type:

     ```bash
     jupyter notebook
     ```

---

## Option 2: Install Jupyter Notebook Standalone

If you prefer not to install Anaconda or Miniconda, you can install Jupyter Notebook directly.

### **Steps to Install Jupyter Notebook via pip**

1. **Install Jupyter Notebook**:
   - Open your Command Prompt and type:

     ```bash
     python -m pip install jupyter
     ```

2. **Launch Jupyter Notebook**:
   - Run the following command to start Jupyter Notebook:

     ```bash
     jupyter notebook
     ```

   - A local server will start, and your browser will open the Jupyter dashboard. Use the provided URL (e.g., `http://localhost:8888/`) if it doesn’t open automatically.

3. **Test Your Setup**:
   - On the Jupyter dashboard, click **New** > **Python 3**.
   - Enter the following code and press **Shift + Enter**:

     ```python
     print("Welcome to Jupyter Notebook!")
     ```

---

## Common Issues and Solutions

<details>
<summary><strong>Theme Errors or Conflicting Packages</strong></summary>

If you see an error like:

```plaintext
AttributeError: module 'notebook.services.contents.filemanager' has no attribute 'themes'
```

Or face other theme-related/package conflicts, follow these steps:

1. Uninstall all Jupyter-related packages:

   ```bash
   pip uninstall jupyter jupyterlab notebook nbconvert nbformat
   ```

2. Clear the pip cache:

   ```bash
   pip cache purge
   ```

3. Reinstall Jupyter Notebook:

   ```bash
   python -m pip install jupyter
   ```
</details>

<details>
<summary><strong>'jupyter' is not recognized as an internal or external command</strong></summary>

This error occurs when the Python Scripts folder is not in your system's PATH.

**Solution**:  
Add the Python Scripts folder (e.g., `C:\Users\YourUsername\AppData\Local\Programs\Python\PythonXX\Scripts`) to your PATH environment variable. Restart Command Prompt after making the changes.
</details>

<details>
<summary><strong>Outdated pip Version</strong></summary>

An outdated pip version can cause installation problems.

**Solution**:  
Upgrade pip by running:

```bash
python -m pip install --upgrade pip
```
</details>

<details>
<summary><strong>Missing Dependencies</strong></summary>

If dependencies are missing during installation:

**Solution**:  
Install required dependencies with:

```bash
python -m pip install --upgrade setuptools wheel
```
</details>

---

## Screenshots

Here are some screenshots to guide you through the process:

![Jupyter Installation Step 1](jupyter_install_ss1.png)  
![Jupyter Installation Step 2](jupyter_install_ss2.png)  

---

## Additional Notes

- **Anaconda Users**: Anaconda is a great starting point for beginners, offering a pre-configured environment for data analysis and machine learning.
- **Miniconda Users**: Miniconda is ideal if you prefer a lightweight setup and want to customize your environment.
- Always ensure Python and pip are up to date for a smoother installation experience.

For more information:  
- [Anaconda Documentation](https://docs.anaconda.com/)  
- [Miniconda Documentation](https://docs.conda.io/en/latest/miniconda.html)  
- [Jupyter Documentation](https://jupyter.org/)  

By following this guide, you’ll have Jupyter Notebook, Anaconda, or Miniconda installed and ready for your data science and machine learning projects. Happy coding!
