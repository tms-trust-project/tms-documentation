..
    Comment: Heirarchy of headers will now be!
    1: ### over and under
    2: === under
    3: --- under
    4: ^^^ under
    5: ~~~ under

.. raw:: html

    <style> .red {color:#FF4136; font-weight:bold; font-size:20px} </style>

.. role:: red

#########################################
Welcome to the Trust Manager System (TMS)
#########################################


What Problem does TMS Address?
==============================

Many research applications and scientific workflows require secure access to distributed resources across multiple organizations. The challenge in automating these workflows is to (1) securely manage user credentials, and (2) execute without human intervention. Automation is primarirly limited by two barriers: securely delegating user credentials across systems and satisfying Multi-Factor Authentication (MFA) requirements without requiring human intervention.  


To address these challenges, the Trust Manager System (TMS) implements authentication and authorization protocols that enable applications to securely connect to host systems on behalf of users and issue commands as those users. TMS is designed to support automated application authentication with four key goals:

   - No manual key distribution
   - No human-in-the-loop, limited duration MFA
   - No secrets shared with applications or users
   - Account access using federated identities

What is TMS?
============

In essence, the Trust Manager System (TMS) provides a manageable way for a science gateway user to authorize and make use of resources at various institutions without having to manually register credentials for each individual resource.

TMS is a multi-tenant web application exposing a REST API to manage SSH keys, client applications, user delegations, user federated identity authentication, resource hosts, and resource host account mappings.

..  TMS includes a module that runs on hosts, such as High Performance Computing (HPC) login nodes, VMs or IoT devices.


.. In its initial incarnation, the **TMS MVP** (Minimal Viable Product) makes a number of simplifying assumptions and implements only a subset of the full API capabilities. This is the TMS version currently available and it's comprised of two components. The **tms_server** web application implements all APIs and maintains state in a Sqlite database. The **KeyCmd** module is a small executable loaded by SSHD that runs on machines into which TMS client applications login on behalf of users.


About This Documentation
========================

.. warning::
  This documentation is under construction.

This documentation includes:

   .. - :doc:`getting-started/index` -- try TMS

   - :doc:`technical/index` -- design and API discussions

   .. - :doc:`deployment/index` -- install TMS components
   .. - :doc:`administration/index` -- maintaining TMS
   
Online Documentation
--------------------

The OpenAPI v3 specification is available here:

   - `API liveDocs`_ -- Interactive API web page

Source code may be found at these links:

   - `TMS Portal source code`_ -- Server github repository
   - `TMS Credential Server source code`_ -- Server github repository
   - `TMS KeyCMD source code`_ -- KeyCMD github repository
   - `TMS Load Tests`_ -- Load test framework

.. _API livedocs: https://tapis-project.github.io/tms-live-docs
.. _TMS Portal source code: https://github.com/tapis-project/tms_portal
.. _TMS Credential Server source code: https://github.com/tapis-project/tms_server
.. _TMS KeyCMD source code: https://github.com/tapis-project/tms_keycmd
.. _TMS Load Tests: https://github.com/tapis-project/tms_loadtest

