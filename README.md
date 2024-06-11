# EXPNext Country Specific Functionality for Kenya

## Includes:

### Kenya Payroll Reports

- P9A Tax Deduction Card
- P10 Tax Report
- NSSF Report
- NHIF Report
- HELB Report
- Bank Payroll Advice Report
- Payroll Register Report

### Tax Reports

- Sales Tax Report
- Purchase Tax Report

---

## P9A Tax Deduction Card Setup

### Salary Component Mapping for P9A

This guide explains the process of mapping salary components to the P9A Tax Deduction Card Type in a Frappe-based system. Follow these steps to configure and manage the salary components effectively.

### Prerequisites

- A Frappe-based application
- Access to the Frappe application
- Basic knowledge of salary components and tax deduction cards

### Step-by-Step Process

#### Access the Frappe Application

1. **Log in to your Frappe instance with your credentials.**

#### Navigate to Salary Component DocType

2. **Go to the DocType list and search for "Salary Component".**
3. **Click on "Salary Component" to view and manage the components.**
   ![Salary Component](image.png)

#### Create New Salary Components

4. **Create a new salary component in the Frappe system.**
5. **Click on "New" to add a new component.**
   ![New Salary Component](image-2.png)

#### Fill in the Salary Component Details

6. **Component Name**: Fill in the component name.
7. **Type**: Choose whether it's an earning or deduction (based on your payroll structure).
8. **P9A Tax Deduction Card Type**: Set this field using the value from the "P9A Tax Deduction Card Type" column.
   ![Component Details](image-1.png)

#### Configure Additional Fields

9. Set other fields like "Do Not Include in Total", "Exempted from Income Tax", "Is Income Tax Component", etc., based on your organizational requirements and the data provided.
   ![Additional Fields](image-3.png)

#### Save the Component

10. Once all relevant fields are filled, **save the new salary component**.
11. Repeat the process for each component.

#### Verify the Components

12. After all components are created, verify that they are correctly mapped and appear as expected in the payroll process.
13. Test the payroll calculations to ensure the formulas are working correctly and the tax deductions are being applied as per the P9A card types.
    ![Verify Components](image-4.png)

### Notes

- Ensure that the formulas are correctly adapted to your Frappe system’s syntax.
- Double-check the P9A tax deduction card types to ensure compliance with your local tax regulations.
- Update the system documentation to reflect any changes made during this process.

## Installation

Using bench, [install ERPNext](https://github.com/frappe/bench#installation) as mentioned here.

Once ERPNext is installed, add CSF_KE app to your bench by running:

```sh
$ bench get-app https://github.com/navariltd/CSF_KE.git
