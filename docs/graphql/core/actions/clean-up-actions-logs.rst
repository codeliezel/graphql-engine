.. meta::
   :description: clean up actions logs
   :keywords: hasura, docs, actions, clean up, async actions

.. _clean_up_actions_logs:

Clean up actions logs
=====================

.. contents:: Table of contents
  :backlinks: none
  :depth: 1
  :local:

Introduction
------------


Table Involved
---------------

Actions have a table managed by Hasura:

- ``hdb_catalog.hdb_action_log``: This is the table that stores all captured logs from asynchronous actions.



Option 1: Get all logs
----------------------

.. code-block:: SQL
   
   SELECT * from hdb_catalog.hdb_action_log;

Option 5: Clear everything
--------------------------

.. code-block:: SQL
   
   DELETE from hdb_catalog.hdb_action_log;