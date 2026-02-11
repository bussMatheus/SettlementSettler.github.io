# Settlement Settler

## Overview

Settlement Settler is a small tool I built to solve a real operational problem I encountered while working at Let Me Be, related to Amazon settlement reconciliation.

Amazon settlement reports provide the final payout amount and a list of individual values (sales, fees, adjustments, etc.), but they don’t always make it clear how those numbers combine to reach the final total. This made it difficult and time-consuming for the team to understand which values were contributing to the final amount.

This tool automates that process.

---

## The Problem

In Amazon settlement spreadsheets:

- You can see multiple values (transactions, fees, refunds, etc.)
- You can see the final total paid by Amazon
- But it's not always clear which combination of values leads to that final number

This created a manual and repetitive task:
- Checking numbers one by one
- Trying to match totals manually
- Wasting time and increasing the risk of mistakes

---

## The Solution

Settlement Settler takes:

- A list of values from the settlement report
- The final total amount

It then uses a backtracking-based approach (similar to the subset sum problem) to:

- Find the exact combination of values that builds the final total
- Return the values that were used to reach that amount

This turns a manual reconciliation task into an automated and reliable process.

---

## Why I'm Proud of This Project

This is not the most complex system I've built, but it's one of the most meaningful because:

- It solved a real business problem
- It was used in a real company environment
- It saved time and reduced manual effort
- It showed how programming can directly improve daily operations

---

## Technical Notes

- Core logic based on backtracking
- Inspired by the classic "subset sum" problem
- Focused on correctness and practical usability

---

## Use Case Example

Input:
- A final settlement total
- A list of transaction values

Output:
- The exact combination of values that sum to the final total

This helps teams understand how the reported total was formed without manually testing combinations.

---

## Author

Matheus Buss  
GitHub: https://github.com/bussMatheus  
LinkedIn: https://www.linkedin.com/in/matheusbuss/

