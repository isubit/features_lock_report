# Features Lock Report
This module will add a section to the site status page at `admin/reports/status` to report on the overall status of feature modules (overridden, locked and overriden, or locked and not overridden). If there are *any* overridden feature components on the site that are not locked it will produce an "error" status. If there is only locked and no overridden feature components it prodoces a "warning" status. Overridden and locked will not trigger an error or warning since they are not a risk of getting reverted during a deployment. The reporting is also available on a component basis at `admin/reports/features-lock`.

# Drush support
This module also includes Drush support to query the status. Run `drush help features-lock-report` for more information.
