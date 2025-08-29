# Reports

Report definitions and templates in hr_attendance.

```mermaid
classDiagram
    class HRAttendanceReport
    Model <|-- HRAttendanceReport
```

## Available Reports

### Analytical/Dashboard Reports
- **Attendance Analysis** (Analysis/Dashboard)


## Report Files

- **hr_attendance_report.py** (Python logic)
- **hr_attendance_report_views.xml** (XML template/definition)
- **__init__.py** (Python logic)

## Notes
- Named reports above are accessible through Odoo's reporting menu
- Python files define report logic and data processing
- XML files contain report templates, definitions, and formatting
- Reports are integrated with Odoo's printing and email systems
