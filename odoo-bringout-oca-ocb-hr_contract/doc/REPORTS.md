# Reports

Report definitions and templates in hr_contract.

```mermaid
classDiagram
    class ContractHistory
    Model <|-- ContractHistory
```

## Available Reports

### Analytical/Dashboard Reports
- **Contracts to Review** (Analysis/Dashboard)
- **Employees** (Analysis/Dashboard)
- **hr.contract.history.list** (Analysis/Dashboard)


## Report Files

- **hr_contract_history.py** (Python logic)
- **hr_contract_history_report_views.xml** (XML template/definition)
- **__init__.py** (Python logic)

## Notes
- Named reports above are accessible through Odoo's reporting menu
- Python files define report logic and data processing
- XML files contain report templates, definitions, and formatting
- Reports are integrated with Odoo's printing and email systems
