# Security

Access control and security definitions in hr_timesheet.

## Access Control Lists (ACLs)

Model access permissions defined in:
- **[ir.model.access.csv](../hr_timesheet/security/ir.model.access.csv)**
  - 7 model access rules

## Record Rules

Row-level security rules defined in:

## Security Groups & Configuration

Security groups and permissions defined in:
- **[hr_timesheet_security.xml](../hr_timesheet/security/hr_timesheet_security.xml)**
  - 4 security groups defined
- **[ir.model.access.xml](../hr_timesheet/security/ir.model.access.xml)**

```mermaid
graph TB
    subgraph "Security Layers"
        A[Users] --> B[Groups]
        B --> C[Access Control Lists]
        C --> D[Models]
        B --> E[Record Rules]
        E --> F[Individual Records]
    end
```

Security files overview:
- **[hr_timesheet_security.xml](../hr_timesheet/security/hr_timesheet_security.xml)**
  - Security groups, categories, and XML-based rules
- **[ir.model.access.csv](../hr_timesheet/security/ir.model.access.csv)**
  - Model access permissions (CRUD rights)
- **[ir.model.access.xml](../hr_timesheet/security/ir.model.access.xml)**
  - Security groups, categories, and XML-based rules

Notes
- Access Control Lists define which groups can access which models
- Record Rules provide row-level security (filter records by user/group)
- Security groups organize users and define permission sets
- All security is enforced at the ORM level by Odoo
