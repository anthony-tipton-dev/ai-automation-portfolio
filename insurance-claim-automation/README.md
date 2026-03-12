# AI-Powered Insurance Claim Processing Automation

**Sprint 7 Final Project** – Demonstrates RPA (UiPath) + AI (LLM prompting) to automate insurance claim extraction, validation, risk analysis, and logging.

### Problem
Manual claim processing causes:
- Slow times
- Data entry errors
- Missed validations
- High costs

### Solution
Automated batch workflow that:
- Extracts data from claim forms using UiPath Document Understanding
- Analyzes for risks/issues using custom LLM prompt (JSON output)
- Validates fields (e.g., diagnosis/procedure codes, totals)
- Handles errors/exceptions with try-catch + email alerts
- Logs structured results (risk level, issues, confidence score) to Google Sheets

### Key Technologies
- UiPath RPA (Document Extraction, Activities, Orchestrator concepts)
- Generative AI / LLM prompting (for risk analysis without predefined models)
- JSON parsing & validation
- Google Sheets integration
- Error handling & data cleaning (remove commas, convert types)

### Workflow Overview
1. Manual trigger + variable init (HighTotalAmount, RiskLevel, etc.)
2. Loop through claim files in folder
3. Extract structured data
4. Send to LLM with strict prompt → returns JSON (riskLevel, issues, confidence, etc.)
5. Validate programmatically (e.g., diagnosis code format)
6. Clean data & handle exceptions
7. Write to Google Sheets via data table + Write Range

<grok-card data-id="6e0b34" data-type="image_card" data-plain-type="render_searched_image"  data-arg-size="LARGE" ></grok-card>



<grok-card data-id="0e0b8e" data-type="image_card" data-plain-type="render_searched_image"  data-arg-size="LARGE" ></grok-card>



<grok-card data-id="f09c7a" data-type="image_card" data-plain-type="render_searched_image"  data-arg-size="LARGE" ></grok-card>


### LLM Prompt Example
Strict JSON-only output with rules for missing fields, fraud signals, format validation (e.g., Claim ID starts with CLM-, etc.).

<grok-card data-id="fedf84" data-type="image_card" data-plain-type="render_searched_image"  data-arg-size="LARGE" ></grok-card>


### Sample Outputs & Validation
Example Google Sheets logging:

<grok-card data-id="6187e0" data-type="image_card" data-plain-type="render_searched_image"  data-arg-size="LARGE" ></grok-card>



<grok-card data-id="156894" data-type="image_card" data-plain-type="render_searched_image"  data-arg-size="LARGE" ></grok-card>


### Issues & Resolutions
- Write Row header glitch → Switched to DataTable + Write Range
- AI inconsistent on diagnosis validation → Handled programmatically

### Benefits
- Faster processing
- Reduced errors
- AI-assisted fraud/risk detection
- Scalable batch handling

### Future Ideas
- Email fraud alerts
- Claims DB integration
- Dashboard reporting
- Webhook triggers

### Resources
- Google Drive folder: [Link](https://drive.google.com/drive/folders/16HjyleCFRGo9hZM9tHw1tvHvxKKA8RqU?usp=drive_link)
- Sample Output Sheet: [Link](https://docs.google.com/spreadsheets/d/1iq0iYZ-H2KISH396eRveE5dK10SbKhBhRz8pkND4Gf4/edit?usp=drive_link)
- Full demo video/slides: [Link](https://drive.google.com/file/d/1eSlCKurm7DUzyCAh95t2MsSdQNcn9ajQ/view?usp=drive_link)
