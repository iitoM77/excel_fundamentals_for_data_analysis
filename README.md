# Excel Fundamentals For Data Analysis
This repo aims to document the excel projects I did in the course

### Module 1 contents: Cleaning and Manipulating data
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


---

### Module 2: working with dates

**Task: Converting date data**
- `=TEXT(A1,"DD/MM/YYYY")` → convert a date to text in day/month/year format
- `=TEXT(A1,"MMMM DD, YYYY")` → convert to full month name format

**Task: Understanding dates**
- `=DAY(A1)`   → returns the day of the month
- `=MONTH(A1)` → returns the month number
- `=YEAR(A1)`  → returns the year
- `=WEEKDAY(A1)` → returns the day of the week (1=Sunday, 2=Monday, etc.)

**Task: Generating valid date using DATE function**
- `=DATE(2026,7,28)` → returns 28 July 2026
- `=DATE(YEAR(A1),MONTH(A1)+1,DAY(A1))` → adds one month to a given date

**Task: Calculations with date**
- `=TODAY()` → current date
- `=NOW()` → current date and time
- `=A1+7` → adds 7 days to a date in cell A1
- `=A1-B1` → difference in days between two dates

**Task: Calculating dates from given dates**
- `=EDATE(A1,1)` → one month after the date in A1
- `=EOMONTH(A1,0)` → last day of the month for the date in A1
- `=DATEDIF(A1,B1,"d")` → number of days between two dates
- `=DATEDIF(A1,B1,"m")` → number of months between two dates
- `=DATEDIF(A1,B1,"y")` → number of years between two dates
- `=NETWORKDAYS(A1,B1)` → number of working days (Mon–Fri) between two dates
- `=NETWORKDAYS(A1,B1,holidays)` → working days excluding specified holidays

---

