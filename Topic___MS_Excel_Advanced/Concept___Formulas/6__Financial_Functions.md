# Financial Functions

| Formula | Description             | Example                   |
| ------- | ----------------------- | ------------------------- |
| `PMT`   | Loan payment            | `=PMT(5%/12, 60, -10000)` |
| `FV`    | Future value            | `=FV(0.05, 10, -1000)`    |
| `PV`    | Present value           | `=PV(0.05, 10, 1000)`     |
| `NPV`   | Net present value       | `=NPV(0.1, A2:A6)`        |
| `IRR`   | Internal rate of return | `=IRR(A2:A6)`             |
| `RATE`  | Interest rate           | `=RATE(60, -100, 5000)`   |

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

### 1. **PMT – Loan Payment**

* **Purpose**:
  Calculates the payment for a loan based on constant payments and a constant interest rate.

* **Syntax**:
  `=PMT(rate, nper, pv, [fv], [type])`

  * `rate`: Interest rate per period (e.g., annual rate divided by 12 for monthly)
  * `nper`: Number of payment periods
  * `pv`: Present value or principal (entered as a negative number for outgoing payments)
  * `[fv]`: Future value (optional; default is 0)
  * `[type]`: Payment timing (0 = end of period, 1 = beginning; optional)

* **Example**:
  `=PMT(5%/12, 60, -10000)`
  → Monthly payment for a \$10,000 loan at 5% annual interest over 5 years

<br/>
<br/>
<br/>

### 2. **FV – Future Value**

* **Purpose**:
  Calculates the future value of an investment based on periodic, constant payments and a constant interest rate.

* **Syntax**:
  `=FV(rate, nper, pmt, [pv], [type])`

  * `rate`: Interest rate per period
  * `nper`: Total number of periods
  * `pmt`: Payment made each period (use negative for outflows)
  * `[pv]`: Present value (optional)
  * `[type]`: Payment timing (optional)

* **Example**:
  `=FV(0.05, 10, -1000)`
  → Value of 10 annual payments of \$1,000 at 5% interest

<br/>
<br/>
<br/>

### 3. **PV – Present Value**

* **Purpose**:
  Calculates the present value of a series of future payments or a lump sum, discounted at a constant interest rate.

* **Syntax**:
  `=PV(rate, nper, pmt, [fv], [type])`

  * `rate`: Interest rate per period
  * `nper`: Total number of periods
  * `pmt`: Payment made each period
  * `[fv]`: Future value (optional)
  * `[type]`: Timing of payment (optional)

* **Example**:
  `=PV(0.05, 10, 1000)`
  → Current worth of 10 annual receipts of \$1,000 at 5% interest

<br/>
<br/>
<br/>

### 4. **NPV – Net Present Value**

* **Purpose**:
  Calculates the net present value of an investment based on a discount rate and a series of future cash flows.

* **Syntax**:
  `=NPV(rate, value1, [value2], ...)`

  * `rate`: Discount rate (interest rate)
  * `value1, value2, …`: Future cash flows (must be equally spaced in time)

* **Note**:
  The initial investment (if any) must be added separately.

* **Example**:
  `=NPV(0.1, A2:A6)`
  → NPV of cash flows in A2 to A6 at a 10% discount rate

<br/>
<br/>
<br/>

### 5. **IRR – Internal Rate of Return**

* **Purpose**:
  Returns the internal rate of return for a series of cash flows (both negative and positive).

* **Syntax**:
  `=IRR(values, [guess])`

  * `values`: Array or range of cash flows (must include at least one negative and one positive value)
  * `[guess]`: Initial guess for the IRR (optional)

* **Example**:
  `=IRR(A2:A6)`
  → IRR for cash flows in A2 to A6

<br/>
<br/>
<br/>

### 6. **RATE – Interest Rate**

* **Purpose**:
  Calculates the interest rate per period of an annuity.

* **Syntax**:
  `=RATE(nper, pmt, pv, [fv], [type], [guess])`

  * `nper`: Total number of payment periods
  * `pmt`: Payment made each period
  * `pv`: Present value (loan amount)
  * `[fv]`: Future value (optional)
  * `[type]`: When payments are due (optional)
  * `[guess]`: Initial guess (optional)

* **Example**:
  `=RATE(60, -100, 5000)`
  → Interest rate for 60 monthly payments of \$100 for a \$5,000 loan
