# Excel Language Translator

A Python script that translates text from an Excel column into another language and saves it in an adjacent column.

## Features
- Reads from Excel files (.xlsx)
- Translates text using Google Translate API
- Preserves original file and creates a new translated version
- Progress tracking during translation
- Error handling for failed translations

## Requirements
openpyxl
googletrans==3.1.0a0

## Installation
1. Clone this repository
2. Install required packages:
pip install -r requirements.txt

## Usage
1. Place your Excel file in the same directory as the script
2. The Excel file should have:
   - Column A: Resource
   - Column B: Primary Language (text to translate)
   - Column C: Translation (where translations will be written)
3. Run the script:
python excel-translator.py

## Example
Check the `examples` directory for sample input and output files:
- `examples/spanish.xlsx`: Sample input file
- `examples/spanish_translated.xlsx`: Sample output file showing translations

### Sample Data Structure:
| Resource ID | Primary Language | Translation |
|-------------|-----------------|-------------|
| greeting_1  | Hello           | Hola        |
| weather_1   | It's sunny      | Está soleado|

## Output
The script creates a new file with '_translated' suffix (e.g., `spanish_translated.xlsx`)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.