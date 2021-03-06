.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.


The following table shows some of the events that may occur during a |chef client| run:

.. list-table::
   :widths: 100 420
   :header-rows: 1

   * - Event
     - Description
   * - ``:audit_phase_failed``
     - |event_type audit_phase_failed|
   * - ``:converge_failed``
     - |event_type converge_failed|
   * - ``:recipe_not_found``
     - |event_type recipe_not_found|
   * - ``:resource_failed``
     - |event_type resource_failed|
   * - ``:run_failed``
     - |event_type run_failed|

The full list of events is available at https://docs.chef.io/dsl_handlers.html#event-types.