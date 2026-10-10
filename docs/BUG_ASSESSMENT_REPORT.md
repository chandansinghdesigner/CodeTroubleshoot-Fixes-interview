# Bug Assessment Report

## Project Overview

Repository: CodeTroubleshoot-Fixes-interview

Source Repository: https://github.com/Ashish-Technocart/CodeTroubleshoot

## 1. Node.js Application

### Bug 1: Book Update Parameters

* **Issue:** Book update parameters were passed in an incorrect order.
* **Impact:** Book fields could be updated with incorrect values.
* **Fix:** Corrected the parameter order.
* **Status:** Fixed; validate with application tests.

### Bug 2: Stock Adjustment Logic

* **Issue:** Negative stock adjustments could incorrectly increase stock.
* **Impact:** Stock quantities could become inaccurate.
* **Fix:** Corrected the stock adjustment calculation.
* **Status:** Fixed; validate positive and negative adjustments.

## 2. Python Application

The Python application was included in the troubleshooting repository. Document each confirmed Python bug here after reviewing the original code and changes.

## Testing

Record the actual test commands, results, and any remaining issues before submission.
