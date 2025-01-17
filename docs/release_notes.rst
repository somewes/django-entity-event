Release Notes
=============

v3.0.0
------
* drop python 3.6
* support python 3.8, 3.9
* django 3.2, 4.0, 4.1

v2.2.1
------
* Fix bad queryset check which would cause it to evaluate. Add explicit None check.

v2.2.0
------
* More optimizations for unseen events
* [!!!BREAKING!!!] Renamed `get_filtered_events_queries` to `get_filtered_events_queryset` on the `Medium` model and it now returns an `Event` queryset

v2.1.0
------
* Optimize querying for unseen events

v2.0.0
------
* Optimize a few querysets
* Add support for django 3.0, 3.1

v1.3.0
------
* Increase model field lengths
* Remove support for django 2.0, 2.1

v1.2.0
------
* Python 3.7
* Django 2.1
* Django 2.2

v1.1.0
------
* Use django's json field with encoder (drop 1.10)

v1.0.0
------
* Add Django 2.0 support
* Use tox for testing more versions
* Bulk create events to save on queries


v0.8.0
------
* Drop Django 1.8 support
* Add Django 1.10 support
* Add Django 1.11 support
* Add python 3.6 support

v0.7.1
------
* Increase the uuid length

v0.7.0
------
* Add creation time for mediums so events can be queried per medium for after medium creation

v0.6.0
------
* Add python 3.5 support, remove django 1.7 support

v0.5.0
------
* Added django 1.9 support

v0.4.4
------
* Added some optimizations during event fetching to select and prefetch some related objects

v0.4.3
------
* Added ability to get a serialized version of an events context data

v0.4.0
------
* Added 1.8 support and dropped 1.6 support for Django

v0.3.4
------
* Fixed django-entity migration dependency for Django 1.6

v0.3.3
------
* Added Django 1.7 compatibility and app config

v0.3.2
------
* Added an additional_context field in the Medium object that allows passing of additional context to event renderings.
* Added ability to define a default rendering style for all sources or source groups if a context renderer is not defined for a particular rendering style.

v0.3.1
------
* Fixes a bug where contexts can have any numeric type as a pk

v0.3.0
------
* Adds a template and context rendering system to entity event

v0.2
----
* This release provides the core features of django-entity-event
  - Event Creation
  - Subscription Management
  - Event Querying
  - Admin Panel
  - Documentation

v0.1
----
* This is the initial release of django-entity-event.
