# 📄 Automatic CV Analysis System

> **Tired of reading hundreds of CVs one by one? Let Python do it for you!**

Built with ❤️ by **Kashi Bhattarai**

---

## 🤔 What Does This Do?

Imagine you're a recruiter and you receive **100 CVs** (resumes) in PDF format. Reading each one manually would take hours. This tool **automates the entire process** — it reads all the CVs automatically, finds the right candidates, and gives you a clean summary in a spreadsheet.

You just point it to a folder of PDFs → it does all the work → you get a neat Excel/CSV file with results. That's it!

---

## ✨ Features

| What it does | How it helps you |
|---|---|
| 📂 Reads all PDF CVs from a folder | No need to open files one by one |
| 🔍 Searches for specific skills | Finds candidates who know Python, Django, MySQL, etc. |
| 📊 Ranks candidates automatically | Best matches appear at the top |
| 📧 Extracts email addresses | Ready to contact shortlisted candidates |
| 📞 Extracts phone numbers | Call them directly from the report |
| 💼 Checks experience level | Filters juniors, mid-level, interns, and more |
| 📁 Saves everything to a CSV file | Open in Excel, Google Sheets — anywhere! |

---

## 🛠️ Skills It Looks For (You Can Customize!)

The tool currently searches for these technical skills in CVs:

```
Python • REST API • Git • HTML • CSS • Java • Django • MySQL • Data
```

And these experience levels:

```
Junior • Mid-level • Entry Level • Internship • Experience
```

> 💡 **Don't worry!** You can easily change these to match whatever skills your company needs. Just edit a simple list in the code.

---

## 🚀 How to Run It

### Step 1 — Install Required Tools

Open your terminal/command prompt and run:

```bash
pip install pdfplumber
```

That's the only external library you need!

### Step 2 — Set Up Your Folder

Put all your CV PDFs into one folder. For example: `E:/csv`

### Step 3 — Update the Folder Path

Open the script and change this one line to match your folder:

```python
folder_path = 'E:/csv'   # ← Change this to your folder
```

### Step 4 — Run the Script

```bash
python python_automatic_cv_analysis.ipynb
```

### Step 5 — Check Your Results

A file called `kashi_output.csv` will appear in your folder. Open it in Excel or Google Sheets!

---

## 📊 What the Output Looks Like

| PDF Name | Matching Words | Experience Level | Total Matches | Email | Phone |
|---|---|---|---|---|---|
| john_doe.pdf | Python, Django, Git | Mid-level | 3 | john@email.com | 984-123-4567 |
| jane_smith.pdf | Python, MySQL | Junior | 2 | jane@email.com | 980-987-6543 |
| bob_jones.pdf | HTML, CSS | Entry Level | 2 | bob@email.com | 985-111-2222 |

> The results are **automatically sorted** — the best-matching candidates are always at the top!

---

## 📁 Files in This Repository

```
📦 automatic_python_CV_analysis-system
 ┣ 📓 python_automatic_cv_analysis.ipynb   ← The main script (Jupyter Notebook)
 ┗ 📊 kashi_output.csv                     ← Sample output file
```

---

## 🧰 Tech Stack

- **Python 3** — The programming language
- **pdfplumber** — Reads text from PDF files
- **re (Regex)** — Finds emails and phone numbers using patterns
- **csv** — Writes the results to a spreadsheet
- **os** — Navigates through your file folders

---

## 💡 Real-World Use Case

This tool is perfect for:

- 🏢 **HR Teams** — Quickly shortlist candidates for a job posting
- 🎓 **Universities** — Screen student internship applications
- 🧑‍💼 **Freelance Recruiters** — Process large volumes of applications fast
- 🏗️ **Startups** — Hire efficiently without a dedicated HR department

---

## ⚙️ Customize It For Your Needs

Want to search for different skills? Just change these lists in the code:

```python
# Add or remove any skills you want to find
target_words = ["RESTAPI", "python", "data", "git", "html", "css", "mysql", "java", "django"]

# Add or remove experience levels
target_sentences = ["experience", "junior", "mid", "Internships", "entrylevel"]
```

---

## 👤 Author

**Kashi Bhattarai**
- GitHub: [@kashi25](https://github.com/kashi25)
- Repository: [automatic_python_CV_analysis-system](https://github.com/kashi25/automatic_python_CV_analysis-system)

---

## 📜 License

This project is open source and free to use. Feel free to fork, modify, and build on top of it!

---

*⭐ If this tool helped you, consider giving it a star on GitHub! It means a lot.*
