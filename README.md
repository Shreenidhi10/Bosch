# **Loading List SMT** 📦🔧

This Flask-based web application provides a secure interface for Bosch employees to validate and mount part numbers. Users can log in, search for specific part numbers in an Excel file, and retrieve SAP and LL values for successful mounting. The app ensures secure authentication and user-friendly workflows.

---

## **Features** 🚀

- **User Authentication:** 
  - Secure login system with pre-defined credentials.
- **Part Number Lookup:** 
  - Search for main and sub-part numbers in an Excel file (`LOADING LIST SMT.xlsx`).
- **SAP and LL Value Retrieval:** 
  - Retrieves SAP and LL values and confirms successful mounting if valid.
- **Error Handling:**
  - Handles errors such as missing columns, invalid inputs, or missing part numbers.
- **Logout Functionality:** 
  - Ensures user sessions are secure and provides an option to log out.

---

## **Prerequisites** 🛠️

1. **Python 3.x**
2. Install the required libraries using pip:
   ```bash
   pip install flask pandas openpyxl
   ```
3. Place the required Excel file (`LOADING LIST SMT.xlsx`) in the project root directory.

---

## **Installation** 🔧

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Bosch.git
   ```

2. Navigate to the project directory:
   ```bash
   cd Bosch
   ```

3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## **Usage** ✨

1. **Start the server**:
   ```bash
   python app.py
   ```

2. Open your browser and navigate to:
   ```
   http://127.0.0.1:5000/
   ```

3. **Login Credentials**:
   ****************
   
5. **Search for Part Numbers**:
   - Enter the **Main Part Number** and **Sub Part Number** to validate.
   - If found, SAP and LL values will be displayed with a success message.

6. **Logout**:
   - Click on the logout button to end the session securely.

---

## **File Structure** 📂

```
part-number-loading-app/
│
├── templates/
│   ├── login.html            # Login page template
│   ├── user.html             # User interface template
│
├── app.py                    # Main application script
└── requirements.txt          # Python dependencies
```

---


## **Error Handling** ⚠️

- **Invalid Login**: Displays an error message for incorrect username or password.
- **Missing Main Part Number**: Error shown if the entered main part number is not found.
- **Missing Sub Part Number**: Error shown if the sub-part number is not listed in the main part's sheet.
- **Excel Errors**: Handles missing columns, incorrect formatting, or file processing errors.

---

## **Enhancements (Future Scope)** 🌟

- **Dynamic User Management**:
  - Add a database for managing user credentials.
- **File Upload Feature**:
  - Allow users to upload their own Excel files dynamically.
- **Advanced Analytics**:
  - Generate reports on frequently accessed part numbers and user activity.
- **Responsive UI**:
  - Enhance the interface for better usability on mobile devices.

---


## **Acknowledgments** 🙏

- **Flask Framework** for enabling quick development of this web app.
- **Pandas Library** for handling Excel file data manipulation.
- Bosch for the inspiration behind the project requirements.
