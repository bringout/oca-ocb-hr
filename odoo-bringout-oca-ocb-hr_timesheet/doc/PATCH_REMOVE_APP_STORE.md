# Patch: Remove App Store Download Links

## Module: hr_timesheet

### Description
This patch removes mobile app store download links (Apple App Store and Google Play Store) from the HR Timesheet configuration settings view.

### Files Modified
- `hr_timesheet/views/res_config_settings_views.xml`

### Changes Made

#### File: hr_timesheet/views/res_config_settings_views.xml
**Lines removed: 59-68**

Removed the following section containing mobile app store download links:
```xml
<div class="col-lg-3 pe-0">
    <a href="https://apps.apple.com/be/app/awesome-timesheet/id1078657549" class="align-middle" target="_blank">
        <img alt="Apple App Store" class="img img-fluid h-100 o_config_app_store" src="project/static/src/img/app_store.png"/>
    </a>
</div>
<div class="col-lg-3 pe-0">
    <a href="https://play.google.com/store/apps/details?id=com.odoo.OdooTimesheets" class="align-middle" target="_blank">
        <img alt="Google Play Store" class="img img-fluid h-100 o_config_play_store" src="project/static/src/img/play_store.png"/>
    </a>
</div>
```

### Impact
- Users will no longer see mobile app store download buttons in the Timesheet configuration settings
- The Chrome Web Store link remains available for users
- The instructional text about tracking time from mobile apps remains intact
- All other timesheet configuration functionality is unaffected

### Context
- The removed links pointed to:
  - Apple App Store: Awesome Timesheet app 
  - Google Play Store: Odoo Timesheets app
- These were displayed in the "Mobile" section of timesheet settings
- The Chrome Web Store option for web-based timesheet access is preserved

### Reason
Removal of proprietary mobile app store references while maintaining the web-based timesheet functionality that doesn't require proprietary app stores.

---
**Patch Created:** 2025-08-27  
**Applied By:** Claude Code Assistant