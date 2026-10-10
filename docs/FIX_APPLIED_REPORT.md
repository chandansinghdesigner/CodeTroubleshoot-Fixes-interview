# Fix Applied Report

## 1. Project Information

* **Assessment:** Code Troubleshooting
* **Candidate:** Chandan Singh
* **Repository:** CodeTroubleshoot-Fixes-interview
* **Applications:** Node.js Book Management API and Python Handwriting Recognition API

## 2. Node.js Application — Fixes Applied

### Bug 1: Incorrect Book Update Parameters

**File:** `bookController.js`

**Problem:** The book update controller passed the price and published year parameters in the wrong order, which could cause incorrect book details to be saved.

**Fix Applied:** Corrected the argument order to match the expected service function parameters.

**Expected Result:** Book details should be updated using the correct price and published year values.

### Bug 2: Incorrect Stock Adjustment Logic

**File:** `stockService.js`

**Problem:** The stock adjustment logic did not correctly handle stock changes and could produce incorrect stock quantities.

**Fix Applied:** Corrected the stock adjustment logic and added appropriate validation for the book ID, book existence, and stock quantity. The logic should prevent invalid adjustments and negative stock.

**Expected Result:** Stock quantities should be updated correctly, and invalid stock adjustments should be rejected.

### Bug 3: Book Repository Delete Operation

**File:** `bookRepository.js`

**Problem:** The delete operation referenced a result variable that was not properly defined in the relevant scope.

**Fix Applied:** Corrected the delete operation to use the actual database operation result and determine whether a record was deleted.

**Expected Result:** The delete operation should complete without a reference error and correctly report whether a book was removed.

### Bug 4: Category Filter Condition

**File:** `bookRepository.js`

**Problem:** The category filter used a not-equal (`!=`) condition, which could return books outside the selected category.

**Fix Applied:** Corrected the filter condition to use equality (`=`), if the intended behavior is to display books matching the selected category.

**Expected Result:** Filtering by category should return books belonging to the selected category.

## 3. Python Application

**Application:** Handwriting Recognition API

The Python application's existing code and test results were reviewed during the assessment. No source-code changes were made because no confirmed issue requiring a code change was identified.

## 4. Testing and Verification

After applying the fixes, the relevant application tests should be executed to verify the changes.

* Node.js tests: Run the configured test command and record the actual result.
* Python tests: Run the configured test command and record the actual result.
* Manual verification: Check book updates, stock adjustments, deletion, and category filtering where applicable.

**Test Results:** Update this section with the actual test commands and results before submitting the report.

## 5. Conclusion

The identified Node.js book management issues were addressed to improve parameter handling, stock adjustment validation, delete-operation reliability, and category filtering. The Python application was reviewed without source-code modifications.

The fixes and test results should be verified against the submitted repository before the assessment is considered complete.
