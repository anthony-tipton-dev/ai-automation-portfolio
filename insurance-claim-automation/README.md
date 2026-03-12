# AI-Powered Insurance Claim Processing Automation

**Sprint 7 Final Project** by Anthony Tipton  
RPA (UiPath) + AI (LLM) automation that extracts, validates, and analyzes insurance claims.

### Problem
Manual claim processing is slow, error-prone, and expensive.

![Challenges](assets/challenges.png)

### Solution & Workflow
Automated batch processing using UiPath Document Understanding + custom LLM prompt.

![Workflow Diagram](assets/workflow-diagram.png)

### Key Steps
1. Initialization & variable setup  
![Initialization](assets/initialization.png)

2. Loop through claim forms  
![For Each File](assets/for-each-loop.png)

3. AI Analysis (LLM Prompt)  
![LLM Prompt](assets/llm-prompt.png)

4. Error Handling & JSON Validation  
![Error Handling](assets/error-handling.png)

5. Data Cleaning & Google Sheets Output  
![Data Cleaning](assets/data-cleaning.png)  
![Google Sheets Example](assets/google-sheets-output.png)

### Example Validation
![Diagnosis Code Example](assets/diagnosis-example.png)

### Benefits
- Faster processing
- Fewer errors
- AI-powered risk & fraud detection
- Scalable for hundreds of claims

![Benefits](assets/benefits.png)

### Future Improvements
![Future Ideas](assets/future-improvements.png)

### Issues & How I Fixed Them
- Write Row glitch → switched to DataTable + Write Range  
- LLM diagnosis validation → handled programmatically  

![Issues Resolved](assets/issues-resolved.png)

### Links
- Full Google Drive folder: https://drive.google.com/drive/folders/16HjyleCFRGo9hZM9tHw1tvHvxKKA8RqU?usp=drive_link  
- Sample Output Google Sheet: https://docs.google.com/spreadsheets/d/1iq0iYZ-H2KISH396eRveE5dK10SbKhBhRz8pkND4Gf4/edit?usp=drive_link  
- Demo video/slides: https://drive.google.com/file/d/1eSlCKurm7DUzyCAh95t2MsSdQNcn9ajQ/view?usp=drive_link

