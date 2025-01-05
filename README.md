**Name:** SHASHANK SATISH MISHRA

**Company:** CODTECH IT SOLUTIONS PVT. LTD

**ID:** CT0806DB

**Domain:** CYBER SECURITY AND ETHICAL HACKING

**Duration:** 3 WEEKS

**Mentor:** NEELA SANTOSH KUMAR

# Overview of the project

# Project: File Integrity Checker


### 1. **Objective**
The primary objective of this project is to create a tool that checks the integrity of files in a specified directory by calculating and displaying their **SHA-256 hashes**. This tool helps ensure that files have not been modified, corrupted, or tampered with by comparing their hash values.

This project aims to:
- Provide a means for users to verify file integrity.
- Support a wide range of file types and directories.
- Provide a simple, user-friendly interface for performing the integrity check.

### 2. **Key Features**
- **Directory Selection**: Users can select a directory from their system to check the integrity of all files inside it.
- **SHA-256 Hash Calculation**: The tool calculates the SHA-256 hash of each file in the selected directory.
- **Results Display**: The calculated hashes are displayed in a scrolled text area, showing each file's path and its corresponding SHA-256 hash.
- **Error Handling**: Provides error messages if files are unreadable, or if the directory does not exist.
- **Simple GUI**: A simple and intuitive graphical interface built using `tkinter`, making it easy for users to interact with the tool.
- **Message Notifications**: The application notifies users of completion or errors via message boxes.

### 3. **How It Works**
1. **User Interaction**: 
   - The user opens the GUI and clicks the "Check Integrity" button.
   - The file dialog allows the user to select the directory to check.

2. **Directory Traversal**:
   - Once a directory is selected, the script walks through all files and subdirectories within it using `os.walk()`.
   - For each file, it opens the file in binary mode and reads the contents in chunks.

3. **Hash Calculation**:
   - The file content is processed in chunks, and the SHA-256 hash is calculated using Python’s built-in `hashlib` library.
   - The hash for each file is displayed in the results area of the GUI.

4. **Results Display**:
   - The calculated SHA-256 hashes for all files in the selected directory are displayed in the scrolled text widget.
   - Upon completion, a message box appears, notifying the user that the integrity check is finished.

### 4. **Components Used**
- **Python**: The core programming language used to develop the script.
- **tkinter**: A standard Python library used for building the graphical user interface (GUI).
- **hashlib**: A built-in Python library used to calculate SHA-256 hashes.
- **os**: Python library used to navigate and handle directories and files.
- **filedialog**: A `tkinter` component that allows users to choose a directory using a graphical file dialog.
- **scrolledtext**: A `tkinter` widget used to display multi-line text with scroll functionality for the output.

### 5. **Application of the Project**
- **File Integrity Verification**: This tool is useful for ensuring that files have not been altered, corrupted, or tampered with. It can be used by developers, system administrators, or security professionals.
- **Backup Validation**: Users can check if their backup files match the originals by comparing their hash values.
- **Data Integrity in Cloud Storage**: It can be used to verify that files stored in cloud services haven’t been changed without the user's knowledge.
- **Software Distribution**: When downloading software or patches from the internet, users can compare the SHA-256 hash of the downloaded file with the official hash to ensure the file is genuine and not tampered with.
- **Compliance and Security**: Organizations can use this tool to ensure that files critical to business operations or security have not been modified.

### 6. **Glimpes of Output**

![image](https://github.com/user-attachments/assets/e1a39450-b8ca-44a2-a83f-ffa12248583e)

![image](https://github.com/user-attachments/assets/577a4427-1fa6-452f-99d6-c195a0704ece)

