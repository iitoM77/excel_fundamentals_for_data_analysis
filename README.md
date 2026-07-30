# Excel Fundamentals For Data Analysis
This repo aims to document the excel projects I did in the course

### Module 1 contents: Introduction, Cleaning and Manipulating text
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

### Module 2: Working with number and dates

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

## Module 3: Defined Names for Working More Effectively with Data

**Task: Cell referencing and naming**
- `=A1` → relative reference
- `=$A$1` → absolute reference
- `=A$1` → mixed reference (fixed row only)
- `=$A1` → mixed reference (fixed column only)

**Task: Define name and create from selection**
- Formulas → Define Name → assign a name
- Formulas → Create from Selection → auto-create names from labels

**Task: Managing named ranges**
- Formulas → Name Manager → view, edit, delete
- Example: `SalesData` refers to `Sheet1!$A$1:$A$10`

**Task: Calculations with named ranges**
- `=SUM(SalesData)`
- `=AVERAGE(Expenses)`
- `=MAX(Revenue)`

**Task: Automation with named ranges**
- `=IF(Total>1000,"Target Met","Target Not Met")`
- `=VLOOKUP(Product,ProductList,2,FALSE)`
- `=INDEX(Prices,MATCH(Item,Items,0))`
- `=XLOOKUP(Product,Items,Prices)`

---

## Module 4: Tables for Automating Data Manipulations

**Task: Creating, naming and removing tables**
- Insert → Table → select range
- Table Design → Table Name → rename
- Right-click → Table → Convert to Range → remove

**Task: Formatting and selecting in tables**
- Table Design → apply styles
- `Ctrl + Space` → select entire column
- `Shift + Space` → select entire row

**Task: Sorting and filtering tables**
- Data → Sort → sort by column
- Data → Filter → apply filters
- Table headers → dropdown filters

**Task: Calculations with structured references**
- `=SUM(Table1[Sales])` → sum of Sales column
- `=AVERAGE(Table1[Expenses])` → average of Expenses column
- `=Table1[@Revenue]` → revenue for current row

**Task: Automating processes with tables**
- Structured references auto-expand with new rows
- Formulas update dynamically when table grows

---

## Module 5: Logical and Lookup Functions

**Task: Performing logical operations with IF**
- `=IF(A1>50,"Pass","Fail")`

**Task: Performing advanced logical operations with nested IFs**
- `=IF(A1>90,"A",IF(A1>80,"B",IF(A1>70,"C","D")))`

**Task: Categorising data with VLOOKUP**
- `=VLOOKUP(ID,DataRange,2,FALSE)` → exact match
- `=VLOOKUP(Score,GradeTable,2,TRUE)` → approximate match

**Task: Matching data with VLOOKUP and XLOOKUP**
- `=VLOOKUP(Product,ProductList,2,FALSE)`
- `=XLOOKUP(Product,Items,Prices)`

**Task: Advanced data matching with INDEX and MATCH**
- `=INDEX(Prices,MATCH(Item,Items,0))`
- `=INDEX(TableRange,MATCH(ID,IDRange,0),2)`
