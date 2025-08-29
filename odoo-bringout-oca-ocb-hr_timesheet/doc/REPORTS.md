# Reports

Report definitions and templates in hr_timesheet.

```mermaid
classDiagram
    class ReportProjectTaskUser
    Model <|-- ReportProjectTaskUser
    class TimesheetsAnalysisReport
    Model <|-- TimesheetsAnalysisReport
```

## Available Reports

### PDF/Document Reports
- **Timesheets** (PDF/Print)
- **Timesheets** (PDF/Print)
- **Timesheets** (PDF/Print)
- **Timesheets** (PDF/Print)

### Analytical/Dashboard Reports
- **Timesheets by Project** (Analysis/Dashboard)
- **Timesheets by Task** (Analysis/Dashboard)


## Report Files

- **hr_timesheet_report_view.xml** (XML template/definition)
- **__init__.py** (Python logic)
- **project_report.py** (Python logic)
- **project_report_view.xml** (XML template/definition)
- **report_timesheet_templates.xml** (XML template/definition)
- **timesheets_analysis_report.py** (Python logic)

## Notes
- Named reports above are accessible through Odoo's reporting menu
- Python files define report logic and data processing
- XML files contain report templates, definitions, and formatting
- Reports are integrated with Odoo's printing and email systems
