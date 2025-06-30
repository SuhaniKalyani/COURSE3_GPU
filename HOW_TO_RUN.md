# How to Run

This document provides instructions on how to run the image processing script in this project.

## Prerequisites

- Python 3.x
- `make` (optional, but recommended for simplicity)

## Quick Start (macOS/Linux)

For macOS and Linux users, the simplest way to run the project is to use the provided shell script. This will handle setting up the virtual environment, installing dependencies, and running the script.

Open your terminal and run the following command from the project root:

```bash
./run.sh
```

## Using Makefile

If you have `make` installed, you can use the `Makefile` to run the project.

1.  **Setup, Install Dependencies, and Run:**
    This single command will set up the virtual environment, install the required packages, and run the main script.

    ```bash
    make
    ```
    or
    ```bash
    make all
    ```

2.  **Clean Up:**
    To remove the virtual environment and all installed packages:
    ```bash
    make clean
    ```

## Manual Setup (All Platforms)

If you prefer to set up the environment manually or you are on Windows, follow these steps.

### 1. Create a Virtual Environment

Navigate to the project directory in your terminal and create a virtual environment.

```bash
python -m venv venv
```

### 2. Activate the Virtual Environment

-   **Windows:**
    ```cmd
    .\venv\Scripts\activate
    ```

-   **macOS/Linux:**
    ```bash
    source venv/bin/activate
    ```

### 3. Install Dependencies

With the virtual environment activated, install the required Python packages.

```bash
pip install --upgrade pip
pip install numpy opencv-python-headless
```

### 4. Run the Script

Once the dependencies are installed, you can run the script.

```bash
python main.py
```

### 5. Deactivate the Virtual Environment

When you are finished, you can deactivate the virtual environment.

```bash
deactivate
```

## Proof of Execution

* Input and Output Folders before and after running the code. (Shown with 3 inputs for example)

![alt text](image.png)
* Running the code.

![alt text](image-1.png)
* Input and Output Folders after running the code.

![alt text](image-2.png)

* Works with multiple inputs as well. 