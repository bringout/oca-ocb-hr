# Patch: Remove App Store Download Links

## Module: hr_expense

### Description
This patch removes mobile app store download links (Apple App Store and Google Play Store) from the HR Expense management interface.

### Files Modified
- `hr_expense/views/hr_expense_views.xml`

### Changes Made

#### File: hr_expense/views/hr_expense_views.xml
**Lines removed: 444-449**

Removed the following section containing mobile app store download links:
```xml
<a href="https://apps.apple.com/be/app/odoo/id1272543640" target="_blank" class="o_expense_mobile_app">
    <img alt="Apple App Store" class="img img-fluid h-100 o_expense_apple_store" src="/hr_expense/static/img/app_store.png"/>
</a>
<a href="https://play.google.com/store/apps/details?id=com.odoo.mobile" target="_blank" class="o_expense_mobile_app">
    <img alt="Google Play Store" class="img img-fluid h-100 o_expense_google_store" src="/hr_expense/static/img/play_store.png"/>
</a>
```

### Impact
- Users will no longer see mobile app store download buttons in the expense management interface
- The promotional text about snapping pictures of receipts remains visible
- The feature description and instructions for mobile expense creation are preserved
- All core expense management functionality remains unchanged

### Context
- The removed links were part of a promotional section encouraging mobile app usage
- Links pointed to:
  - Apple App Store: Official Odoo mobile app
  - Google Play Store: Official Odoo mobile app  
- The section was visible on desktop browsers (`d-none d-md-block` class)
- The instructional text "Snap pictures of your receipts and let Odoo automatically create expenses for you" remains

### Reason
Removal of proprietary mobile app store references while maintaining the informational content about mobile expense features that can be accessed through web browsers or alternative app distribution methods.

---
**Patch Created:** 2025-08-27  
**Applied By:** Claude Code Assistant