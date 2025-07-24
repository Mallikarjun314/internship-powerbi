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




<br/><br/><br/><br/>

## 1. **VLOOKUP**

#### **Description and Purpose**

`VLOOKUP` (Vertical Lookup) searches for a value in the first column of a range and returns a value in the same row from a specified column.

<br/><br/>

```=VLOOKUP(lookup_value,table_array, col_index_num, [range_lookup])```

<br/><br/>

| Field            | Description                                                     |
| ---------------- | --------------------------------------------------------------- |
| `lookup_value`   | The value to search for in the first column of the table        |
| `table_array`    | The range containing the data to search                         |
| `col_index_num`  | The column number in the range from which to return a value     |
| `[range_lookup]` | Optional: TRUE for approximate match (default), FALSE for exact |

#### **Usage Example**

```xlsx
=VLOOKUP(101, A2:C10, 2, FALSE)
```
→ Looks for `101` in column A and returns corresponding value from column B.


<br/><br/><br/><br/>

## 2. **HLOOKUP**

#### **Description and Purpose**

`HLOOKUP` (Horizontal Lookup) searches for a value in the first row of a range and returns a value from a specified row in the same column.

<br/><br/>

`=HLOOKUP(lookup_value, table_array, row_index_num, [range_lookup])`

<br/><br/>

| Field            | Description                                               |
| ---------------- | --------------------------------------------------------- |
| `lookup_value`   | The value to search for in the first row of the table     |
| `table_array`    | The range of cells to search within                       |
| `row_index_num`  | The row number (starting from 1) to return the value from |
| `[range_lookup]` | Optional: TRUE = approximate match, FALSE = exact match   |

#### **Usage Example**

```xlsx
=HLOOKUP("Q1", A1:D3, 2, FALSE)
```
→ Looks for "Q1" in row 1 and returns value from row 2 in the same column.


<br/><br/><br/><br/>

## 3. **INDEX**

#### **Description and Purpose**

`INDEX` returns the value at a specific position in a range based on row and column numbers.

<br/><br/>

`=INDEX(array, row_num, [column_num])`

<br/><br/>

| Field          | Description                                       |
| -------------- | ------------------------------------------------- |
| `array`        | Range of cells or array from which to return data |
| `row_num`      | Row number in the array                           |
| `[column_num]` | Optional: Column number (if array is 2D)          |

#### **Usage Example**

```xlsx
=INDEX(A1:C3, 2, 3)
```
→ Returns value from 2nd row and 3rd column (i.e., cell C2)


<br/><br/><br/><br/>

## 4. **MATCH**

#### **Description and Purpose**

`MATCH` returns the position of a value in a row or column.

<br/><br/>

`=MATCH(lookup_value, lookup_array, [match_type])`

<br/><br/>

| Field          | Description                                                          |
| -------------- | -------------------------------------------------------------------- |
| `lookup_value` | The value you want to find                                           |
| `lookup_array` | The range of cells to search                                         |
| `[match_type]` | Optional: 0 = exact, 1 = less than, -1 = greater than (default is 1) |

#### **Usage Example**

```xlsx
=MATCH(50, A1:A10, 0)
```
→ Returns position of value `50` in range A1\:A10


<br/><br/><br/><br/>

## 5. **XLOOKUP**

#### **Description and Purpose**

`XLOOKUP` is a modern replacement for `VLOOKUP` and `HLOOKUP`, allowing search in any direction with easier syntax and more control.

<br/><br/>

`=XLOOKUP(lookup_value, lookup_array, return_array, [if_not_found], [match_mode], [search_mode])`

<br/><br/>

| Field            | Description                                                         |
| ---------------- | ------------------------------------------------------------------- |
| `lookup_value`   | The value to search for                                             |
| `lookup_array`   | The array/range to search within                                    |
| `return_array`   | The range to return values from                                     |
| `[if_not_found]` | Optional: Value to return if not found                              |
| `[match_mode]`   | Optional: 0 = exact, -1/1 = next smaller/larger, 2 = wildcard match |
| `[search_mode]`  | Optional: 1 = first to last, -1 = last to first                     |

#### **Usage Example**

`=XLOOKUP("Apple", A2:A10, B2:B10, "Not Found")`
→ Returns matching value from B2\:B10 where A2\:A10 contains "Apple"


<br/><br/><br/><br/>

## 6. **CHOOSE**

#### **Description and Purpose**

`CHOOSE` returns a value from a list based on a given index number.

<br/><br/>

`=CHOOSE(index_num, value1, [value2], ...)`

<br/><br/>

| Field        | Description                             |
| ------------ | --------------------------------------- |
| `index_num`  | Position of the value to return         |
| `value1...n` | List of values or ranges to choose from |

#### **Usage Example**

`=CHOOSE(2, "Red", "Blue", "Green")`
→ Returns `"Blue"` because it’s the 2nd item.


<br/><br/><br/><br/>

## 7. **LOOKUP**

#### **Description and Purpose**

`LOOKUP` searches for a value in a range and returns a corresponding value from another range.

<br/><br/>

`=LOOKUP(lookup_value, lookup_vector, [result_vector])`

<br/><br/>

| Field             | Description                                                |
| ----------------- | ---------------------------------------------------------- |
| `lookup_value`    | The value to search for                                    |
| `lookup_vector`   | One-row or one-column range to search                      |
| `[result_vector]` | Optional: Range to return value from (same size as lookup) |

#### **Usage Example**

`=LOOKUP(25, A1:A5, B1:B5)`
→ Finds 25 in A1\:A5 and returns the corresponding value from B1\:B5
