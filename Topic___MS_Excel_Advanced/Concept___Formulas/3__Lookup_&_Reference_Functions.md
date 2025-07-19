# Lookup & Reference Functions

| Formula   | Description              | Example                              |
| --------- | ------------------------ | ------------------------------------ |
| `VLOOKUP` | Vertical lookup          | `=VLOOKUP(101, A2:B10, 2, FALSE)`    |
| `HLOOKUP` | Horizontal lookup        | `=HLOOKUP("Jan", A1:D3, 2, FALSE)`   |
| `INDEX`   | Returns value at row/col | `=INDEX(A1:C3, 2, 2)`                |
| `MATCH`   | Position of value        | `=MATCH(25, A1:A10, 0)`              |
| `XLOOKUP` | Advanced lookup          | `=XLOOKUP("John", A2:A10, B2:B10)`   |
| `CHOOSE`  | Chooses from list        | `=CHOOSE(2, "Red", "Blue", "Green")` |
| `LOOKUP`  | Approximate match        | `=LOOKUP(4, A1:A10, B1:B10)`         |
