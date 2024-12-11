# LocalizationConverter
A script which takes and excel file and generates new localized files for the languages choosen

Usage:

To run the given Python script and translate your Excel file, follow these steps:

1. Save the Script
Copy the entire code into a file and save it with a .py extension, for example, translate_excel.py.
2. Prepare Your Excel File
Place the Excel file (translations.xlsx in this case) in the same directory as the script.
Ensure the columns you want to translate contain text (e.g., English phrases) and are formatted correctly.
The first row should typically be a header row, and translation will start from the second row.
3. Customize Parameters
Modify the parameters at the bottom of the script:

python
Copy code
file_path = "translations.xlsx"  # Replace with the path to your Excel file
columns_to_translate = [1, 3]    # Replace with the 1-based column numbers you want to translate
source_lang = "en"               # Replace with the source language code (e.g., "en" for English)
target_langs = ["es", "fr", "de"]             # Replace with the target language code (e.g., "es" for Spanish)
replace = true                  # Set to True if you want to replace the existing columns
For example:

To translate columns A and C (1, 3) from English to French, set:
python
Copy code
columns_to_translate = [1, 3]
source_lang = "en"
target_langs = ["es", "fr", "de"]
4. Run the Script
Open a terminal or command prompt, navigate to the folder containing translate_excel.py, and run:

bash
Copy code
python translate_excel.py
5. Check the Output
If the script runs successfully, the translated file will be saved in the same folder as the input file with a name like translations_es.xlsx (for Spanish).
The new file will contain the translations either in new columns or as replacements, based on the replace flag.
