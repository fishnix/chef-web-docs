.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

This resource has the following properties:

.. list-table::
   :widths: 150 450
   :header-rows: 1

   * - Property
     - Description
   * - ``admin``
     - |admin client|
   * - ``chef_server``
     - |chef_server_url|
   * - ``complete``
     - Use to specify if this resource defines a user completely. When ``true``, any property not specified by this resource will be reset to default property values.
   * - ``email``
     - The email address for the user.
   * - ``external_authentication_uid``
     - 
   * - ``ignore_failure``
     - **Ruby Types:** TrueClass, FalseClass

       |ignore_failure| Default value: ``false``.
   * - ``name``
     - The name of the user.
   * - ``notifies``
     - **Ruby Type:** Symbol, 'Chef::Resource[String]'

       |notifies|

       .. include:: ../../includes_resources_common/includes_resources_common_notifications_syntax_notifies.rst

       .. include:: ../../includes_resources_common/includes_resources_common_notifications_timers.rst
   * - ``output_key_format``
     - Use to specify the format of a public key. Possible values: ``pem``, ``der``, or ``openssh``. Default value: ``openssh``.
   * - ``output_key_path``
     - Use to specify the path to the location in which a public key will be written.
   * - ``raw_json``
     - The user as |json| data. For example:
       
       .. code-block:: javascript
       
          {
            "name": "Robert Forster"
          }
   * - ``recovery_authentication_enabled``
     - 
   * - ``retries``
     - **Ruby Type:** Integer

       |retries| Default value: ``0``.
   * - ``retry_delay``
     - **Ruby Type:** Integer

       |retry_delay| Default value: ``2``.
   * - ``source_key``
     - Use to copy a public or private key, but apply a different ``format`` and ``password``. Use in conjunction with ``source_key_pass_phrase``` and ``source_key_path``.
   * - ``source_key_pass_phrase``
     - The pass phrase for the public key. Use in conjunction with ``source_key``` and ``source_key_path``.
   * - ``source_key_path``
     - The path to the public key. Use in conjunction with ``source_key``` and ``source_key_pass_phrase``.
   * - ``subscribes``
     - **Ruby Type:** Symbol, 'Chef::Resource[String]'

       |subscribes|

       .. include:: ../../includes_resources_common/includes_resources_common_notifications_syntax_subscribes.rst

       |subscribes timers|
