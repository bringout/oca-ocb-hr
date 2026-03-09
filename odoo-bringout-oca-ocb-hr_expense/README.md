# Expenses


Manage expenses by Employees
============================

This application allows you to manage your employees' daily expenses. It gives you access to your employees’ fee notes and give you the right to complete and validate or refuse the notes. After validation it creates an invoice for the employee.
Employee can encode their own expenses and the validation flow puts it automatically in the accounting after validation by managers.


The whole flow is implemented as:
---------------------------------
* Draft expense
* Submitted by the employee to his manager
* Approved by his manager
* Validation by the accountant and accounting entries creation

This module also uses analytic accounting and is compatible with the invoice on timesheet module so that you are able to automatically re-invoice your customers' expenses if your work by project.
    

## Installation

```bash
pip install odoo-bringout-oca-ocb-hr_expense
```

## Dependencies

- account
- web_tour
- hr

## Source

- Repository: https://github.com/OCA/OCB
- Branch: 19.0
- Path: addons/hr_expense

## License

This package preserves the original LGPL-3 license.
