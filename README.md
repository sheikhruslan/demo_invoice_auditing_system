# Invoice Auditing System

## Overview

This project aims to develop a Python program that assists in the auditing process for the sales and invoice system at AI_Tone Mall. The program is designed to create an audit file that checks the correctness of transactions and the integrity of data stored in the system.

## Features

1. **Invoice Number Validation**: Ensures the format of the invoice number is correct.
2. **Order Number Verification**: Validates the correctness of the order number displayed in the invoice record, including the check digit.
3. **Cost Verification**:
   - Calculates the subtotal and total payment.
   - Verifies the correctness of discounts applied (VIP and VVIP discounts).
   - Determines the delivery fee based on the subtotal.
4. **Hash Total Calculation**: Computes the hash total for the order for inventory checking.
5. **Mall Dollars Calculation**: Calculates mall dollars based on the total payment if it meets the specified threshold.

## Detailed Description

- **Invoice Format**: The program checks that the invoice number follows a specific format, including a combination of letters and digits.
- **Check Digit Calculation**: It uses the staff number as a multiplier and applies a modulus to compute the check digit for order verification.
- **Cost Breakdown**: It calculates the subtotal, applies any discounts, and adds the delivery fee to determine the total cost.
- **Hash Total**: The hash total is the sum of the last two digits of item numbers in the order, used for further processing.
- **Mall Dollars**: If the total payment meets or exceeds $1000, the program calculates the mall dollars as a percentage of the total.

## Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/AI_Tone_Mall_Invoice_Auditing_System.git
   ```
   
2. Navigate to the project directory:
   
   ```bash
   cd AI_Tone_Mall_Invoice_Auditing_System
   ```
   
3. Open the Jupyter Notebook:
   
   ```bash
   jupyter notebook invoice_auditing_system.ipynb
   ```
   
