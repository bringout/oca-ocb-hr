# Time Off


Manage time off requests and allocations
========================================

This application controls the time off schedule of your company. It allows employees to request time off. Then, managers can review requests for time off and approve or reject them. This way you can control the overall time off planning for the company or department.

You can configure several kinds of time off (sickness, paid days, ...) and allocate time off to an employee or department quickly using time off allocation. An employee can also make a request for more days off by making a new time off allocation. It will increase the total of available days for that time off type (if the request is accepted).

You can keep track of time off in different ways by following reports:

* Time Off Summary
* Time Off by Department
* Time Off Analysis

A synchronization with an internal agenda (Meetings of the CRM module) is also possible in order to automatically create a meeting when a time off request is accepted by setting up a type of meeting in time off Type.


## Installation

```bash
pip install odoo-bringout-oca-ocb-hr_holidays
```

## Dependencies

- hr
- calendar
- resource

## Source

- Repository: https://github.com/OCA/OCB
- Branch: 19.0
- Path: addons/hr_holidays

## License

This package preserves the original LGPL-3 license.
