Keeping code bloat to a minimum is a high priority. Thus, we create custom builds of components that allow this.

## jQuery UI

jQuery UI is a big library. We use only these components:

### UI Core

* Core
* Widget
* Mouse

### Interactions

* Draggable

### Widgets

* Datepicker
* Tabs

## Moment.js

We need language files for Moment.js but using all of them makes the javascript file too big.

Only the languages needed, are included in these files:

* de.js
* es.js
* fr.js
* id.js
* pl.js
* pt.js
* ru.js
* zh-cn.js

