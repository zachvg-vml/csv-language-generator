# CSV Language Generator Web Tool

A secure, client-side web tool that helps you quickly generate multiple versions of a CSV file for different languages.

## Tool Available on Github Pages
https://zachvg-vml.github.io/csv-language-generator/

## 🚀 What this tool does

This tool allows you to take a master CSV file (for example, a contact list or a translation file) and automatically duplicate it for a list of target languages.

1.  **Takes an input CSV.**
2.  **Identifies the "Original" language** from the first row of data.
3.  **Creates a copy** of the original file, renaming it to include the language (e.g., `contacts_English.csv`).
4.  **Generates new CSVs** for every target language you list (e.g., `contacts_Spanish.csv`, `contacts_Korean.csv`), automatically updating the specific language column inside the file.
5.  **Zips everything** into a single download package.

## ✨ Features

*   **100% Client-Side:** All processing happens in your browser. Your CSV data is **never** uploaded to any server, ensuring complete data privacy.
*   **No Backend Required:** Runs entirely on HTML, CSS, and JavaScript.

## 🛠️ How to use

1.  Open the `index.html` file in your browser (or visit the hosted page).
2.  **Upload Source CSV:** Select your `.csv` file. It must have headers in the first row.
3.  **Language Column Header:** Type the exact name of the column header that contains the language (default is `language_written`).
4.  **Target Languages:** Edit the list of languages you want to generate files for (one per line).
5.  **Generate:** Click the button. The tool will process the files and automatically download a `processed_languages.zip` file.

## 🌐 How to host on GitHub Pages

Since this tool is a single HTML file, it is incredibly easy to host for free using GitHub Pages.

### Step 1: Create a Repository
1.  Log in to [GitHub](https://github.com).
2.  Click the **+** icon in the top right and select **New repository**.
3.  Name your repository (e.g., `csv-language-generator`).
4.  Make sure it is set to **Public**.
5.  Click **Create repository**.

### Step 2: Upload the Code
1.  On your computer, ensure you have the `index.html` file saved.
2.  On the GitHub repository page, click the link that says **uploading an existing file**.
3.  Drag and drop your `index.html` file into the box.
4.  In the "Commit changes" box at the bottom, type "Initial commit".
5.  Click **Commit changes**.

### Step 3: Enable GitHub Pages
1.  Click on the **Settings** tab at the top of your repository.
2.  In the left sidebar, look for the **Code and automation** section and click on **Pages**.
3.  Under **Build and deployment** > **Branch**:
*   Select `main` (or `master`) from the dropdown menu.
*   Ensure the folder is set to `/(root)`.
4.  Click **Save**.

### Step 4: Access your Tool
Wait about 1-2 minutes for GitHub to build your site. refresh the Pages settings page. You will see a banner at the top saying:

> **Your site is live at `https://<your-username>.github.io/csv-language-generator/`**

Click that link to use your tool!

## 📦 Libraries Used

*   **[PapaParse](https://www.papaparse.com/):** The fastest in-browser CSV (or delimited text) parser for JavaScript.
*   **[JSZip](https://stuk.github.io/jszip/):** A library for creating, reading and editing .zip files with JavaScript.