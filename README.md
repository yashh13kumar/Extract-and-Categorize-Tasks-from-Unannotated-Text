 Extract and Categorize Tasks from Unstructured Text

 Overview
This project processes unstructured text to extract and categorize tasks based on predefined categories. It uses Natural Language Processing (NLP) techniques with spaCy and regular expressions to identify tasks, deadlines, and classify them accordingly.

 Features
- Extracts task-related phrases (e.g., "needs to", "should", "must").
- Detects deadlines like "by 5 pm", "tomorrow", or "within 3 days" using regex.
- Categorizes tasks into domains such as Personal, Academic, Work, Household, Health, and Finance.

 Technologies Used
- Python
- spaCy (for NLP processing)
- Regular Expressions (re module) (for deadline extraction)
- JSON (for structured output)

 Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/extract-tasks.git
   cd extract-tasks
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Download the spaCy English model:
   ```bash
   python -m spacy download en_core_web_sm
   ```

 Usage
1. Run the script to analyze a sample text:
   ```bash
   python main.py "John needs to submit the assignment by tomorrow and call the doctor."
   ```
2. Example output:
   ```json
   {
       "tasks": [
           {"task": "submit the assignment", "category": "Academic", "deadline": "tomorrow"},
           {"task": "call the doctor", "category": "Health", "deadline": "N/A"}
       ]
   }
   ```

 File Structure
- `main.py` - The main script to process text input.
- `task_extraction.py` - Handles task extraction logic.
- `requirements.txt` - Lists dependencies.
- `README.md` - Documentation.

 Future Enhancements
- Improve deadline detection with more robust NLP models.
- Expand task categories dynamically using machine learning.
- Implement a web or API interface for better usability.

 Contributions
Feel free to contribute by submitting pull requests or issues for improvements!


