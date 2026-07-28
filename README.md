# Excel Fundamentals For Data Analysis
This repo aims to document the excel projects I did in the course

### Module 1 contents:
**Task: Combining text data**
- `=CONCATENATE(A1, " ", B1)`
- `=TEXTJOIN(" ", TRUE, A1, B1)`
- `=A1 & " " & B1`

**Task: Splitting text data**
- `=LEFT(A1,5)`   → first 5 characters
- `=RIGHT(A1,3)`  → last 3 characters
- `=MID(A1,3,4)`  → 4 characters starting at position 3
- `=TEXTSPLIT(A1,",")`  → split by comma (Excel 365/2021)

**Task: Combining text functions**
- `=LEFT(A1,3) & RIGHT(B1,2)`
- `=PROPER(CONCATENATE(A1," ",B1))`

**Task: Cleaning data**
- `=TRIM(A1)`   → remove extra spaces
- `=CLEAN(A1)`  → remove non-printable characters
- `=PROPER(A1)` → capitalize each word
- `=UPPER(A1)`  → all caps
- `=LOWER(A1)`  → all lowercase

**Task: Replacing text characters**
- `=REPLACE(A1,2,3,"XYZ")` → replace 3 chars starting at position 2
- `=SUBSTITUTE(A1,"old","new")` → replace all occurrences of "old" with "new"

### Module 1 project
- [Module 1](Projects/Module 1)
- 
