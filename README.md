# Ding Event Automatic Unpublishing
Module created for automatic un-publishing of expired event nodes.

On the event creation/updating, the scheduler's "Unpublish on" field will be automatically populated by event's end
date/time plus some buffer (configured in module's settings), so once it's expired - node will be un-published by Drupal
scheduler functionality.

### Installation:
1. Go to ```/admin/modules```
2. Enable ```Ding Event Automatic Unpublishing``` module and click "Save configuration" button

or

Enable module via drush: ```drush en -y ding_event_unpublishing```

### Configuration:
Module's configuration is available at ```/admin/config/ding_event/settings``` page.
In order to enable automatic unpublishing functionality, the configuration option ```Enable event un-publish scheduling```
must be checked.
Down below this option, will appear the text field for filling the time buffer which will be added to the event's end
time in hours.
Default will be "0", so the un-publish time will be the same as node's end time.
