# Growth Mindset Challenge: Python Web App using Streamlit

## 📌 Project Overview
### Purpose
Growth Mindset File Transformer is a **Streamlit web app** designed to help users **upload, clean, filter, visualize, and convert** data files (CSV, Excel) effortlessly. This tool also provides AI-powered suggestions to enhance data quality, embodying the **growth mindset** philosophy—the belief that skills and abilities improve through effort and learning.

## ✨ Features
- **📂 File Upload**: Supports **CSV and XLSX** formats. Accepts multiple files at once.
- **🛠 Data Cleaning**:
  - Remove **duplicate** rows.
  - Fill missing values using **mean-based imputation**.
- **📊 Data Selection & Filtering**:
  - Select specific **columns** to work with before conversion.
  - Interactive **visualization** using **bar charts**.
- **🔄 Data Conversion**:
  - Convert cleaned data to **CSV or Excel** formats.
  - Download processed files with a single click.

---

## 🚀 Getting Started
### Prerequisites
Make sure you have the following installed:
- **Python 3.7+**
- Required Python packages:
  - `streamlit`
  - `pandas`
  - `openpyxl`
  - Other dependencies (see `requirements.txt`)

### 🔧 Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/growth-mindset-file-transformer.git
   cd growth-mindset-file-transformer
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

### ▶️ Running the App
Start the Streamlit app using:
```sh
streamlit run app.py
```

---

## 📝 Code Overview
### `app.py`
This script:
1. **Uploads** CSV or Excel files.
2. **Previews** the uploaded data.
3. **Performs data cleaning**:
   - Removes duplicates.
   - Fills missing values (numeric columns only).
4. **Allows column selection**.
5. **Generates bar charts** for numeric data.
6. **Converts data** to CSV or Excel and allows downloading.

### Key Functions Used:
- `st.file_uploader()`: Uploads multiple files.
- `pd.read_csv()` / `pd.read_excel()`: Reads files into a DataFrame.
- `df.drop_duplicates()`: Removes duplicate rows.
- `df.fillna(df.mean())`: Fills missing numeric values.
- `st.multiselect()`: Allows users to select columns.
- `st.bar_chart()`: Displays a bar chart for numeric columns.
- `df.to_csv()` / `df.to_excel()`: Converts data for download.

---
## 🛠 Future Enhancements
- ✅ AI-powered data cleaning suggestions (via Gemini API).
- ✅ Additional file format support (e.g., JSON, XML, Parquet).
- ✅ More advanced data transformation options.

## 🤝 Contributing
Contributions are welcome! If you'd like to contribute:
1. **Fork** the repository.
2. **Create** a new branch (`git checkout -b feature-branch`).
3. **Commit** changes (`git commit -m "Added new feature"`).
4. **Push** to the branch (`git push origin feature-branch`).
5. **Create a Pull Request**.

## 📜 License
This project is licensed under the **MIT License**.

---


🔹 *Embrace the growth mindset and transform your data effortlessly!* 🚀

