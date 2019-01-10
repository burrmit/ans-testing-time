Ansible Time Testing Playbook
============================================
 Version | Date Modified | Editor  | Comments
---------|---------------|---------|-------------------
1.0      | 10 JAN 2019   | m.burr  | Intial version

Overview
-------------
This playbook is to test out being able to control when a playbook is able to be executed.  This is done by getting
the time using the ansible_date_time module to get it from localhost, then creating a pre_task that ends the playbook
if executed at a specific time.

The example used here is, if the playbook is not run on Thursday between 8:30pm and 8:59pm then it will not execute.
