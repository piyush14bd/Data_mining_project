### **README.md**  

# **Setting Up a Python Virtual Environment in VS Code**  

## **Prerequisites**  
Ensure you have:  
- **Python** installed ([Download](https://www.python.org/downloads/))  
- **VS Code** installed ([Download](https://code.visualstudio.com/))  
- **Git** installed ([Download](https://git-scm.com/))  
- **Python extension** installed in VS Code  

---

## **Step 1: Clone the GitHub Repository**  
Before setting up the virtual environment, clone your project from GitHub:  

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
```

---

## **Step 2: Create a Virtual Environment**  
Inside the cloned repository, run:  

```bash
python -m venv .venv
```
This creates a virtual environment named **`venv`**.

---

## **Step 3: Activate the Virtual Environment**  
### **Windows (PowerShell)**
```bash
venv\Scripts\Activate
```
### **Mac/Linux**
```bash
source venv/bin/activate
```

---

## **Step 4: Select the Virtual Environment in VS Code**  
1. Press **`Ctrl + Shift + P`** (or `Cmd + Shift + P` on Mac).  
2. Search for **"Python: Select Interpreter"**.  
3. Choose the one inside **`venv`** (e.g., `.venv/bin/python`).  

---

## **Step 5: Install Dependencies**  
If your project has dependencies listed in **requirements.txt**, install them:  
```bash
pip install -r requirements.txt
```
To save installed packages for future use:  
```bash
pip freeze > requirements.txt
```

---

## **Step 6: Deactivate the Virtual Environment**  
Exit the virtual environment by running:  
```bash
deactivate
```

---

## **IGNORE STEPS 4,5 and 6.**


## **Troubleshooting**  
- If `venv\Scripts\Activate` is not working on Windows, run:  
  ```bash
  Set-ExecutionPolicy Unrestricted -Scope Process
  ```

---

## **Conclusion**  
You have successfully:  
✅ Cloned your GitHub repository.  
✅ Set up a **Python virtual environment** in **VS Code**.  
✅ Installed dependencies and configured the workspace.  

Now, you can start coding in an isolated environment! 🚀  

Would you like a script to automate this setup? 😃
