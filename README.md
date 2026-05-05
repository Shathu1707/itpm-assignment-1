ITPM Assignment 1 – Functional and Usability Testing

Project Overview

This project is part of the IT3040 – ITPM Semester 1 module.
The objective of this assignment is to perform **functional and usability testing** on the website:

https://www.pixelssuite.com/

The testing focuses on verifying whether the system behaves correctly under normal conditions and whether the user interface is easy to use.

Features Tested

The following features were tested:

* Document Conversion
* PDF Editing
* Image Resizing
* Image Cropping
* Compression
* Image Format Conversion
* Meme Generator
* Color Picker
* Image Rotation
* Image Flipping

---

Testing Approach

Manual Testing

 36 test cases were created
 Each feature includes:

  * 1 Positive test case
  * 2 Negative test cases
* Additional 6 test cases were included

---

 Automation Testing (Playwright)

* One test case was automated using **Playwright (Python)**
* Scenario tested:

  * Upload a PNG image
  * Verify preview functionality

---

 Prerequisites

Make sure the following are installed:

* Python 3.11 or 3.12
* Google Chrome (or Chromium)

---

 Installation Steps

Run the following commands:

```bash
pip install -U pip
pip install playwright openpyxl
playwright install
```

---

 How to Run the Test

Navigate to the project folder:

```bash
cd /d D:\test_automation_ui
```

Run the Playwright script:

```bash
python image_preview_test.py --url "https://www.pixelssuite.com/convert-to-png" --slow-mo-ms 2000
```

---

 Expected Output

After running the script:

* ✔ Browser opens automatically
* ✔ PNG image is uploaded
* ✔ Preview is displayed
* ✔ Test result is recorded

---

Output Files

### 1. CSV File

`execution_results.csv`

Contains:

* Test name
* Status (PASS/FAIL)

---

### 2. Screenshot

`results/preview_pass.png`

* Captured when preview is successfully detected

---

 Test Result

* Preview detected: **True**
* Status: **PASS**

---

 Project Structure

```
test_automation_ui/
│
├── image_preview_test.py
├── execution_results.csv
├── sample.png
├── results/
│   └── preview_pass.png
```

---

 Notes

* Only frontend functionality and usability were tested
* Backend, performance, and security testing were not included
* Assumptions were made for expected outputs where necessary

---

 Author

* Name: Shathukshan J
* Registration Number: IT23563346

---
