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

Many research applications and scientific workflows require secure access to distributed resources across multiple
organizations. The challenge in automating these workflows is to (1) securely manage user credentials, and (2) use
those credentials to execute commands on the resources without human intervention. Automation is primarirly limited
by two barriers: securely delegating user credentials across systems and satisfying Multi-Factor Authentication (MFA)
requirements without requiring human intervention.

To address these challenges, the Trust Manager System (TMS) implements authentication and authorization protocols
that enable applications to securely connect to host systems on behalf of users and issue commands as those users.
TMS is designed to support automated application authentication with four key goals:

   - No manual key distribution
   - Limited duration MFA with no human-in-the-loop
   - No secrets shared with applications or users
   - Account access using federated identities

What is TMS?
============

In essence, the Trust Manager System (TMS) provides a manageable way for an application user to authorize and make
use of resources at various institutions without having to manually register credentials for each individual resource.
An example of a typical application would be a science gateway web application.

TMS is a web application exposing a REST API to manage SSH keys, client applications, user delegations, user federated
identity authentication, resource hosts, and resource host account mappings.


About This Documentation
========================

.. warning::
  This documentation is under construction.

This documentation includes:

   - :doc:`technical/index` -- design and API discussions
   
Online Documentation
--------------------

The OpenAPI v3 specification is available here:

   - `API liveDocs`_ -- Interactive API web page

Source code may be found at these links:

   - `TMS Portal source code`_ -- Server github repository
   - `TMS Credential Server source code`_ -- Server github repository
   - `TMS KeyCMD source code`_ -- KeyCMD github repository
   - `TMS Load Tests`_ -- Load test framework

.. _API livedocs: https://tms-trust-project.github.io/tms-live-docs
.. _TMS Portal source code: https://github.com/tms-trust-project/tms_portal
.. _TMS Credential Server source code: https://github.com/tms-trust-project/tms_server
.. _TMS KeyCMD source code: https://github.com/tms-trust-project/tms_keycmd
.. _TMS Load Tests: https://github.com/tms-trust-project/tms_loadtest

