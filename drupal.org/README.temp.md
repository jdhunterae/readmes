Contents of this File
=====

[TOC]

Introduction
-----

The Administration Menu module displays the entire administrative menu tree (and most local tasks) in a drop-down menu, providing administrators one- or two-click access to most pages. Other modules may also add menu links to the menu using `hook_admin_menu_output_alter()`.

* For a full description of the module, visit the page:
	https://drupal.org/project/admin_menu

* To submit bug reports and feature suggestions, or to track changes:
	https://drupal.org/project/issues/admin_menu

Requirements
-----

This module requires the following modules:

* Views (https://drupal.org/project/views)
* Panels (https://drupal.org/project/panels)

Recommended Modules
-----

* Markdown filter (https://drupal.org/project/markdown):
	When enabled, display of the project's README.md help will be rendered with markdown.

Installation
-----

* Install as you would normally install a contributed Drupal module. See: https://drupal.org/documentation/install/modules-themes/modules-7 for more information.

* You may want to disable Toolbar module, since its output clashes with Administration Menu.

Configuration (alt: some)
-----

* Configure user permissions in Administration &raquo; People &raquo; Permissions:

  * Use the administation pages and help (System module)

    The top-level administration categories require this permission to be accessible. The administration menu will be empty unless this permission is granted.

  * Access administration menu

    Users in roles with the "Access administration menu" permission will see the administration menu at the top of each page.

  * Display Drupal links

    Users in roles with the "Display Drupal links" permission will recieve links to drupal.org issue queues for all enabled contributed modules. The issue queue links will appear under the administration menu icon.

* Customize the menu settings in Administration &raquo; Configuration and modules &raquo; Administration &raquo; Administration menu.

* To prevent administrative menu items from appearing twice, you may hide the "Management" menu block.

Configuration (alt: none)
-----

The module has no menu or modifiable settings. There is no configuration. When enabled, the module will prevent the links from appearing. To get the links back, disable the module and clear caches.

Troubleshooting
-----

* If the menu does not display, check the following:

  * Are the "Access administration menu" and "Use the administration pages and help" permissions enabled for the appropriate roles?
  * Does html.tpl.php of your theme output the `$page_bottom` variable?

FAQ
-----

Q: I enabled "Aggregate and compress CSS files", but admin_menu.css is still there. Is that normal?

A: Yes, this is the intended behavior. The administration menu module only loads its stylesheet as needed (i.e., on page requests by logged-on administrative users).


MAINTAINERS
-----

Current maintainers:
* Daniel F. Kudwien (sun) - https://drupal.org/user/54136
* Peter Wolanin (pwolanin) - https://drupal.org/user/49851
* Stefan M. Kudwien (smk-ka) - https://drupal.org/user/48898
* Dave Reid (Dave Reid) - https://drupal.org/user/53892

This project has been sponsored by:
* UNLEASHED MIND
	Specialized in consulting and planning of Drupal powered sites, UNLEASHED MIND offers installation, development, theming, customization, and hosting to get you started. Visit https://www.unleashedmind.com for more information.