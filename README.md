# TRACE AI
### Test Requirements Automation and Case Engine

> Built by a Systems Engineer, for Systems Test Engineers. Upload your requirements. Get your full test documentation in minutes.

---

<img width="1661" height="628" alt="image" src="https://github.com/user-attachments/assets/8e5029e3-bcc8-4da2-889c-2be75d4c3c75" />

---

## What is this?

Writing test cases from scratch takes hours. Reading through requirements, figuring out what to test, formatting everything into a test plan, building a traceability matrix... it adds up fast.

TRACE AI takes your requirements document and does all of that for you. You upload the file, select the requirements you want to cover, hit Generate, and it produces four things:

1. **System Study** - an initial analysis of what the system does and what testing it needs
2. **Test Plan** - a structured plan covering test scope, schedule, environments and responsibilities
3. **Test Cases** - detailed, executable test cases with steps and expected results for every requirement
4. **Traceability Matrix** - a complete RTM mapping every requirement to its test cases

Everything is readable inside the app and downloadable as a file.

---

## Quick look

<img width="350" height="453" alt="image" src="https://github.com/user-attachments/assets/a5bc5aee-d1a7-4509-8780-a31e6108f12b" />

*Upload your file, name your project, and choose what to generate*

---

## How it works

**Step 1: Upload your requirements**

The app accepts PDF, DOCX, TXT and Excel files. The Excel format works best. Use three columns: Requirement ID, Requirement Text, Test Scenario.

<img width="1545" height="850" alt="image" src="https://github.com/user-attachments/assets/20b4072b-8c3e-4398-9915-ee6ea4b1a1ca" />

**Step 2: Select requirements**

Every requirement from your document shows up as a checkbox. You pick which ones to include. Select all, or just the ones relevant to your current sprint.

<img width="1290" height="786" alt="image" src="https://github.com/user-attachments/assets/4334a8bd-0f1e-4a9d-891a-359bcbc3f18b" />

**Step 3: Generate**

Click Generate. The app calls the Claude API and streams each section live so you can watch it build in real time.

<img width="1515" height="582" alt="image" src="https://github.com/user-attachments/assets/c691db67-a6ed-45d4-87ba-2c1e1f81e90b" />

**Step 4: Review and download**

Each of the four sections opens in its own tab. The content is fully formatted with tables, headers and numbered steps. Download individual sections or the full report as a single file.

<img width="1540" height="508" alt="image" src="https://github.com/user-attachments/assets/89b304c4-b422-4b02-b825-03a14d95cc0b" />

---

## The four outputs

### System Study

This is the first thing any test engineer should produce before writing a single test case. TRACE AI generates a scope document, a risk assessment and entry and exit criteria based purely on reading your requirements.

<img width="1542" height="849" alt="image" src="https://github.com/user-attachments/assets/5a76077a-f668-47e4-9c1a-903612c0721d" />

### Test Plan

Covers test objectives, test types (functional, regression, performance, security), environment setup, a schedule table and a resource plan. Follows the IEEE 829 standard structure.

<img width="1165" height="904" alt="image" src="https://github.com/user-attachments/assets/4d6fd159-c5af-457c-a347-810d9b63e08d" />

---

<img width="979" height="635" alt="image" src="https://github.com/user-attachments/assets/9d00d1eb-2a2f-4272-846c-242c4126993e" />

### Test Cases

For every requirement, you get positive test cases, a negative test case and at least one edge case. Each one has a test case ID, a mapped requirement ID, preconditions, step by step actions, expected results and pass/fail criteria.

<img width="1444" height="717" alt="image" src="https://github.com/user-attachments/assets/67ac8e67-f843-40e7-ab06-ba9f7a24dd45" />

### Traceability Matrix

A forward traceability table (requirement to test case) and a backward traceability table (test case back to requirement), plus a coverage summary showing percentage of requirements covered.

<img width="1461" height="933" alt="image" src="https://github.com/user-attachments/assets/b29c727c-4189-4ac5-afb9-10d79b3c01af" />

---

## Who this is for?

This tool was built to support the early stages of the Software Testing Life Cycle (STLC). If you spend more time formatting documentation than actually thinking about test coverage, this is for you.

It works well for:

- Automotive and embedded systems QA where requirements documents are long and structured
- Agile teams who need test documentation fast at the start of a sprint
- Engineers starting on a new project who need to get up to speed on what needs testing
- Anywhere you have a formal SRS or requirements sheet and need to go from requirements to test cases quickly

---

## Sample requirements file

A sample Excel requirements sheet for an FM Radio infotainment feature is as shown. It has 10 requirements across functional and non-functional categories, ready to upload and test the tool with.

<img width="1054" height="683" alt="image" src="https://github.com/user-attachments/assets/a2cc2be0-080b-4e48-be14-baddef78a92a" />

---

## Tech used

- Python and Streamlit for the interface
- Claude Sonnet via the Anthropic API for generation
- pdfplumber and python-docx for file parsing
- openpyxl for Excel support
- All outputs are Markdown so they paste cleanly into Confluence, Notion or any wiki

---

## What this is not

This does not replace a QA engineer. The generated test cases are a strong starting point for someone starting on a new project without functional experience but they still need to be reviewed, adjusted for your actual test environment, and expanded based on what you know about the system that is not in the requirements document. Think of it as doing the first draft for you.

---

*TRACE AI was built as a personal productivity tool for QA work. Feedback and contributions welcome.*
