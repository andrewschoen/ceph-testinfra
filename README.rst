==============
ceph-testinfra
==============

A collection of tests that are used to verify ceph cluster
are running as expected. This uses the testinfra_ project
as the basis for the tests. Originally these tests were ported
from the ceph-volume_ and ceph-ansible_ projects.

This project assumes you'll use the ansible backend of testinfra
and that ansible config will give provided for the following.

.. code-block:: yaml
   
   public_interface: eno1
   cluster_interface: eno1
   public_network: 10.8.129.0/24
   num_osds: 1
   is_containerized: False


.. _testinfra: https://testinfra.readthedocs.io/en/latest/
.. _ceph-volume: https://github.com/ceph/ceph
.. _ceph-ansibel: https://github.com/ceph/ceph-ansible
