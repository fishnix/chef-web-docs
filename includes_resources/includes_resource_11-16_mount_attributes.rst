.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

This resource has the following properties:

.. list-table::
   :widths: 150 450
   :header-rows: 1

   * - Property
     - Description
   * - ``device``
     - **Ruby Type:** String

       Required for ``:umount`` and ``:remount`` actions (for the purpose of checking the mount command output for presence). |device mount|
   * - ``device_type``
     - **Ruby Type:** Symbol

       |device_type| Default value: ``:device``.
   * - ``domain``
     - **Ruby Type:** String

       |windows| only. Use to specify the domain in which the ``username`` and ``password`` are located.
   * - ``dump``
     - **Ruby Types:** Integer, FalseClass

       |dump_frequency| Default value: ``0``.
   * - ``enabled``
     - **Ruby Types:** TrueClass, FalseClass

       Use to specify if a mounted file system is enabled. Default value: ``false``.
   * - ``fstype``
     - **Ruby Type:** String

       Required. |fstype|
   * - ``ignore_failure``
     - **Ruby Types:** TrueClass, FalseClass

       |ignore_failure| Default value: ``false``.
   * - ``mount_point``
     - **Ruby Type:** String

       |mount_point| |resource_block_default| |see syntax|
   * - ``mounted``
     - **Ruby Types:** TrueClass, FalseClass

       Use to specify if a file system is already mounted. Default value: ``false``.
   * - ``notifies``
     - **Ruby Type:** Symbol, 'Chef::Resource[String]'

       |notifies|

       .. include:: ../../includes_resources_common/includes_resources_common_notifications_syntax_notifies.rst

       .. include:: ../../includes_resources_common/includes_resources_common_notifications_timers.rst
   * - ``options``
     - **Ruby Types:** Array, String

       |options mount| Default value: ``defaults``.
   * - ``pass``
     - **Ruby Types:** Integer, FalseClass

       |pass_number| Default value: ``2``.
   * - ``password``
     - **Ruby Type:** String

       |windows| only. Use to specify the password for ``username``.
   * - ``provider``
     - **Ruby Type:** Chef Class

       Optional. |provider resource_parameter| |see providers|
   * - ``retries``
     - **Ruby Type:** Integer

       |retries| Default value: ``0``.
   * - ``retry_delay``
     - **Ruby Type:** Integer

       |retry_delay| Default value: ``2``.
   * - ``subscribes``
     - **Ruby Type:** Symbol, 'Chef::Resource[String]'

       |subscribes|

       .. include:: ../../includes_resources_common/includes_resources_common_notifications_syntax_subscribes.rst

       |subscribes timers|
   * - ``supports``
     - **Ruby Type:** Array

       |supports mount| Default value: ``{ :remount => false }``.
   * - ``username``
     - **Ruby Type:** String

       |windows| only. Use to specify the user name.
