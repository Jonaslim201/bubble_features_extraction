To run the notebook,
---
### 1. Prerequisites
Ensure you have the UV package manager installed.
https://docs.astral.sh/uv/
```bash
pip install uv
```
Ensure Jupyter extension is installed in VSC.

---
### 2. Create virtual environment
In the root folder, run
```bash
uv venv
```
---
### 3. Activate the venv using
**Windows:**
```bash
.venv/Scripts/activate
```
---
**MacOS/Linux:**
```bash
source .venv/bin/activate
```
---
### 4. Installing dependencies
While the venv is active, download all the relevant packages using:
```bash
uv sync
```
---
## Jupyter Notebook Setup (VSCode)

### 5. Select Kernel

1. Open the `.ipynb` file
2. Click on the kernel selector in the top-right corner
3. Select the virtual environment you just created

### Troubleshooting

If the kernel isn't visible:

1. **Refresh Available Kernels:**
   - Click the refresh button next to "Select a Python Environment" in the top bar

2. **Manually Select Python Interpreter:**
   - Press `Cmd+Shift+P` (Mac) or `Ctrl+Shift+P` (Windows/Linux)
   - Type: `Python: Select Interpreter`
   - Look for your venv
   - If not found, proceed to step 3

3. **Enter Interpreter Path Manually:**
   - Press `Cmd+Shift+P` (Mac) or `Ctrl+Shift+P` (Windows/Linux)
   - Type: `Python: Select Interpreter`
   - Click **"Enter interpreter path..."**
   
   **Paste the appropriate path:**
   - **MacOS/Linux:** `.venv/bin/python`
   - **Windows:** `.venv\Scripts\python.exe`
   
4. **Change Kernel:**
   - Try selecting the kernel again in the notebook
   - It should now appear in the list
