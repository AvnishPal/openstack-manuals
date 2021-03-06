..
    Warning: Do not edit this file. It is automatically generated from the
    software project's code and your changes will be overwritten.

    The tool to generate this file lives in openstack-doc-tools repository.

    Please make any changes needed in the code, then run the
    autogenerate-config-doc tool from the openstack-doc-tools repository, or
    ask for help on the documentation mailing list, IRC channel or meeting.

.. _neutron-lbaas_agent:

.. list-table:: Description of LBaaS agent configuration options
   :header-rows: 1
   :class: config-ref-table

   * - Configuration option = Default value
     - Description
   * - **[DEFAULT]**
     -
   * - ``debug`` = ``False``
     - (Boolean) If set to true, the logging level will be set to DEBUG instead of the default INFO level.
   * - ``device_driver`` = ``['neutron_lbaas.drivers.haproxy.namespace_driver.HaproxyNSDriver']``
     - (Multi-valued) Drivers used to manage loadbalancing devices
   * - ``interface_driver`` = ``None``
     - (String) The driver used to manage the virtual interface.
   * - ``periodic_interval`` = ``40``
     - (Integer) Seconds between running periodic tasks
   * - **[haproxy]**
     -
   * - ``loadbalancer_state_path`` = ``$state_path/lbaas``
     - (String) Location to store config and state files
   * - ``send_gratuitous_arp`` = ``3``
     - (Integer) When delete and re-add the same vip, send this many gratuitous ARPs to flush the ARP cache in the Router. Set it below or equal to 0 to disable this feature.
   * - ``user_group`` = ``nogroup``
     - (String) The user group
