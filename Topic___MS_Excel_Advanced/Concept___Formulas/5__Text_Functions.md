# Text Functions

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
