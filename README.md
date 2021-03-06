bootstrap-collapse-clickchange
==============================

Extends the Bootstrap Collapse jQuery plugin to allow automatic changing of both the target and parent element in the DOM.

**Version 1.0.2**

Usage
-------

Simply add `data-click="clickchange"` to the parent element.
For groups, this is the parent element.
For standalone collapses it is the clickable element.
See the demo page for instructions and code.

To have an individual collapse within a group behave differently, treat that collapse as a standalone.
The standalone settings will completely over-ride any group settings, so these may need to be reset.

The classes that are changed are toggled using jQuery's `toggleClass()`. Therefore both on and off classes need to be defined.

Options
-------

These options can be passed through data elements or directly on invocation. e.g. data-<option-name>

* **when**: ( *before*|start) When to change trigger the changes. This will tie into the show/shown and hide/hidden events
* **targetclass**: ( *null*|string) The classes to toggle on the container of the collapsible content.
* **parentclass**: ( *null*|string) The classes to toggle on the clickable element that shows/hides the collapsible content.
* **iconchange**: (true| *false*) Change icons within the clickable element
* **iconclass**: ( *null*|string): The classes to change on the icon elements. e.g. `chevron-up chevron-down`
* **iconprefix**: ( *glyphicon*|string) The icon prefix. Used to target which icons to change. e.g. The default will find all elements with a class of glyphicon to change
* **iconprefixadd**: ( *true*|false) Whether to append this icon-prefix to the passed icon classes. If it is, a '-' character is added before the class names

To do
-------

Change Log
-------

### 1.0.2

* Calling code for a grouping now works as expected (Issue 1)
* The pluging now works in IE8 (Issue 3)
* Updated default settings to match readme, to make the plugin more generic (Issue 2)
* Refactored code based on JSHint
* Fixed typo on demonstration page

### 1.0.1

* Fixed bug where events were propogating up to the parent collapse
* Added more examples

