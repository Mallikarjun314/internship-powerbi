# MS-Excel Important Formulas and Functions

## 🔢 **1. Mathematical Functions**

| Formula     | Description                  | Example                 |
| ----------- | ---------------------------- | ----------------------- |
| `SUM`       | Adds numbers together        | `=SUM(A1:A5)`           |
| `SUBTOTAL`  | Returns subtotal for a range | `=SUBTOTAL(9, A1:A10)`  |
| `PRODUCT`   | Multiplies numbers           | `=PRODUCT(A1:A3)`       |
| `ROUND`     | Rounds to specified digits   | `=ROUND(A1, 2)`         |
| `ROUNDUP`   | Rounds number up             | `=ROUNDUP(3.1416, 2)`   |
| `ROUNDDOWN` | Rounds number down           | `=ROUNDDOWN(3.1416, 2)` |
| `INT`       | Rounds down to integer       | `=INT(5.9)`             |
| `MOD`       | Returns remainder            | `=MOD(10,3)`            |
| `POWER`     | Raises to power              | `=POWER(2,3)`           |
| `SQRT`      | Square root                  | `=SQRT(16)`             |

---

## 🧠 **2. Logical Functions**

| Formula   | Description                  | Example                     |
| --------- | ---------------------------- | --------------------------- |
| `IF`      | Conditional logic            | `=IF(A1>10, "High", "Low")` |
| `IFERROR` | Custom value for errors      | `=IFERROR(A1/B1, "Error")`  |
| `AND`     | Returns TRUE if all are TRUE | `=AND(A1>0, B1<10)`         |
| `OR`      | Returns TRUE if any are TRUE | `=OR(A1=1, B1=2)`           |
| `NOT`     | Reverses logical value       | `=NOT(A1=5)`                |
| `IFS`     | Multiple conditions          | `=IFS(A1>90,"A",A1>80,"B")` |

---

## 🔍 **3. Lookup & Reference Functions**

| Formula   | Description              | Example                              |
| --------- | ------------------------ | ------------------------------------ |
| `VLOOKUP` | Vertical lookup          | `=VLOOKUP(101, A2:B10, 2, FALSE)`    |
| `HLOOKUP` | Horizontal lookup        | `=HLOOKUP("Jan", A1:D3, 2, FALSE)`   |
| `INDEX`   | Returns value at row/col | `=INDEX(A1:C3, 2, 2)`                |
| `MATCH`   | Position of value        | `=MATCH(25, A1:A10, 0)`              |
| `XLOOKUP` | Advanced lookup          | `=XLOOKUP("John", A2:A10, B2:B10)`   |
| `CHOOSE`  | Chooses from list        | `=CHOOSE(2, "Red", "Blue", "Green")` |
| `LOOKUP`  | Approximate match        | `=LOOKUP(4, A1:A10, B1:B10)`         |

---

## 📅 **4. Date & Time Functions**

| Formula       | Description            | Example                 |
| ------------- | ---------------------- | ----------------------- |
| `TODAY`       | Current date           | `=TODAY()`              |
| `NOW`         | Current date & time    | `=NOW()`                |
| `DATE`        | Creates date           | `=DATE(2025, 7, 18)`    |
| `EDATE`       | Adds months to date    | `=EDATE(A1, 3)`         |
| `EOMONTH`     | End of month           | `=EOMONTH(A1, 1)`       |
| `DAY`         | Day of month           | `=DAY(A1)`              |
| `MONTH`       | Month number           | `=MONTH(A1)`            |
| `YEAR`        | Year from date         | `=YEAR(A1)`             |
| `DATEDIF`     | Date difference        | `=DATEDIF(A1, B1, "y")` |
| `NETWORKDAYS` | Workdays between dates | `=NETWORKDAYS(A1, B1)`  |
| `WEEKDAY`     | Day of week            | `=WEEKDAY(A1, 2)`       |

---

## 🧾 **5. Text Functions**

| Formula                  | Description                       | Example                         |
| ------------------------ | --------------------------------- | ------------------------------- |
| `CONCATENATE` / `CONCAT` | Joins strings                     | `=CONCAT(A1, " ", B1)`          |
| `TEXTJOIN`               | Joins with delimiter              | `=TEXTJOIN(", ", TRUE, A1:A3)`  |
| `LEFT`                   | Extracts left characters          | `=LEFT(A1, 5)`                  |
| `RIGHT`                  | Extracts right characters         | `=RIGHT(A1, 4)`                 |
| `MID`                    | Extracts from middle              | `=MID(A1, 3, 4)`                |
| `LEN`                    | Length of text                    | `=LEN(A1)`                      |
| `FIND`                   | Finds position (case-sensitive)   | `=FIND("e", A1)`                |
| `SEARCH`                 | Finds position (case-insensitive) | `=SEARCH("e", A1)`              |
| `TRIM`                   | Removes extra spaces              | `=TRIM(A1)`                     |
| `UPPER`                  | Converts to uppercase             | `=UPPER(A1)`                    |
| `LOWER`                  | Converts to lowercase             | `=LOWER(A1)`                    |
| `PROPER`                 | Capitalizes words                 | `=PROPER(A1)`                   |
| `REPLACE`                | Replaces part of string           | `=REPLACE(A1, 1, 3, "XYZ")`     |
| `SUBSTITUTE`             | Replaces specific text            | `=SUBSTITUTE(A1, "old", "new")` |

---

## 💰 **6. Financial Functions**

| Formula | Description             | Example                   |
| ------- | ----------------------- | ------------------------- |
| `PMT`   | Loan payment            | `=PMT(5%/12, 60, -10000)` |
| `FV`    | Future value            | `=FV(0.05, 10, -1000)`    |
| `PV`    | Present value           | `=PV(0.05, 10, 1000)`     |
| `NPV`   | Net present value       | `=NPV(0.1, A2:A6)`        |
| `IRR`   | Internal rate of return | `=IRR(A2:A6)`             |
| `RATE`  | Interest rate           | `=RATE(60, -100, 5000)`   |

---

## 📊 **7. Statistical Functions**

| Formula      | Description                  | Example                                   |
| ------------ | ---------------------------- | ----------------------------------------- |
| `AVERAGE`    | Mean                         | `=AVERAGE(A1:A10)`                        |
| `MEDIAN`     | Middle value                 | `=MEDIAN(A1:A10)`                         |
| `MODE`       | Most frequent                | `=MODE.SNGL(A1:A10)`                      |
| `MAX`        | Maximum                      | `=MAX(A1:A10)`                            |
| `MIN`        | Minimum                      | `=MIN(A1:A10)`                            |
| `COUNT`      | Count numbers                | `=COUNT(A1:A10)`                          |
| `COUNTA`     | Count non-empty cells        | `=COUNTA(A1:A10)`                         |
| `COUNTBLANK` | Count empty cells            | `=COUNTBLANK(A1:A10)`                     |
| `COUNTIF`    | Count with condition         | `=COUNTIF(A1:A10, ">10")`                 |
| `COUNTIFS`   | Count with multiple criteria | `=COUNTIFS(A1:A10, ">10", B1:B10, "<20")` |

---

## 🛠️ **8. Array / Dynamic Functions (New Excel)**

| Formula     | Description                     | Example                         |
| ----------- | ------------------------------- | ------------------------------- |
| `UNIQUE`    | Returns unique values           | `=UNIQUE(A1:A10)`               |
| `SORT`      | Sorts values                    | `=SORT(A1:A10)`                 |
| `FILTER`    | Filters data                    | `=FILTER(A1:B10, B1:B10="Yes")` |
| `SEQUENCE`  | Creates sequence                | `=SEQUENCE(5)`                  |
| `RANDARRAY` | Returns array of random numbers | `=RANDARRAY(3,2)`               |

---

## 🧮 **9. Engineering/Conversion Functions**

| Formula   | Description       | Example                     |
| --------- | ----------------- | --------------------------- |
| `CONVERT` | Unit conversion   | `=CONVERT(100, "km", "mi")` |
| `DEC2BIN` | Decimal to binary | `=DEC2BIN(10)`              |
| `BIN2DEC` | Binary to decimal | `=BIN2DEC(1010)`            |
