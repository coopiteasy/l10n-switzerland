=====================
Switzerland - Payroll
=====================

.. !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
    :target: https://odoo-community.org/page/development-status
    :alt: Beta
.. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
    :alt: License: AGPL-3
.. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fl10n--switzerland-lightgray.png?logo=github
    :target: https://github.com/OCA/l10n-switzerland/tree/11.0/l10n_ch_hr_payroll
    :alt: OCA/l10n-switzerland
.. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
    :target: https://translation.odoo-community.org/projects/l10n-switzerland-11-0/l10n-switzerland-11-0-l10n_ch_hr_payroll
    :alt: Translate me on Weblate
.. |badge5| image:: https://img.shields.io/badge/runbot-Try%20me-875A7B.png
    :target: https://runbot.odoo-community.org/runbot/125/11.0
    :alt: Try me on Runbot

|badge1| |badge2| |badge3| |badge4| |badge5| 

[ This file must be max 2-3 paragraphs, and is required. ]

Switzerland Payroll Rules
=========================

This module allows you to manage the salaries of your employees

** Features list :**
    * Add Swiss salary rule categories
    * Add Swiss salary rules
    * Add children in school to employee
    * Add LPP range to contract
    * Add LPP Amount to contract.
    * Add Holiday Rate to contract.

** For further information:**
    * Payroll accounting: http://open-net.ch/blog/la-comptabilite-salariale-suisse-avec-odoo-1/tag/salaires-6

** Remarks: **
    * To prevent overwriting your salary rules changes, an update from 1.0.8 and lower to 1.0.9 and higher creates duplicates of the salary rules. This is because with some migrated databases, one may encounter a difficulty with the existing rules (they can not be erased if they are already used). The solution is then to force the existing ones to be non-updatable. And this is done using an included pre-migration script.
    * As this module proposes its own report (same as the original, but with its own footer), don't forget to make it non-updatable.
    * If you choose to uninstall this module, you have to manually delete the rules.

**Table of contents**

.. contents::
   :local:

Installation
============

[ This file must only be present if there are very specific
  installation instructions, such as installing non-python
  dependencies. The audience is systems administrators. ]

To install this module, you need to:

#. Do this ...

Configuration
=============

[ This file is optional, it should explain how to configure
  the module before using it; it is aimed at advanced users. ]

To configure this module, you need to:

#. Go to ...

.. figure:: https://raw.githubusercontent.com/OCA/l10n-switzerland/11.0/l10n_ch_hr_payroll/path/to/local/image.png
   :alt: alternative description
   :width: 600 px

Usage
=====

[ This file must be present and contains the usage instructions
  for end-users. As all other rst files included in the README,
  it MUST NOT contain reStructuredText sections
  only body text (paragraphs, lists, tables, etc). Should you need
  a more elaborate structure to explain the addon, please create a
  Sphinx documentation (which may include this file as a "quick start"
  section). ]

To use this module, you need to:

#. Go to ...

Changelog
=========

[ The change log. The goal of this file is to help readers
  understand changes between version. The primary audience is
  end users and integrators. Purely technical changes such as
  code refactoring must not be mentioned here. 
  
  This file may contain ONE level of section titles, underlined
  with the ~ (tilde) character. Other section markers are 
  forbidden and will likely break the structure of the README.rst
  or other documents where this fragment is included. ]


V1.0.0: 2014-11-07/Sge
    * Add Salary rule categories.
    * Add Salary rules.
    * Add Employee children in school.
    * Add Contract LPP rate.

V1.0.1: 2014-11-11/Sge
    * Set the 'LPP rate'' digits to 'Payroll Rate' decimal accuracy.

V1.0.2:
    * Add some minor changes, based on pull request #66 comments.

V1.0.3-4:
    * Add LPP Amount to contract.
    * Add Worked Hours Rate to contract.
    * Add Hourly Rate to contract.
    * Compute the Wage of contract, based on Worked Hours and Hourly Rate.
    * Add new salay rules

V1.0.5:
    * Add Holiday Rate to contract.
    * Update "Indemnité vacances 8,33%" rule to include
      "Holiday Rate" from contract.

V1.0.6:
    * Move salary rules from CSV file to XML file.
    * Import salary rules only at install.
    * Internal reorganization of files (.py and .xml).

V1.0.7:
    * Added: two new dependencies (hr_contract and hr_attendance)

V1.0.8:
    * Updated: the "Appears on slip" settings
    * Integrated: report for the payslip, with its own footer
    * Added: a pre-migration script
    * pre-migration script correctly set

V1.1:
    * New: commissions and reimbursements management in pay slips and contracts

V1.2:
    * Journal entries generated by the confirmation of a payslip now inherits correctly of the partner's name
V1.3:
    * Move commission and reimbursement management to hr_payroll_commission and hr_payroll_expense modules

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/l10n-switzerland/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us smashing it by providing a detailed and welcomed
`feedback <https://github.com/OCA/l10n-switzerland/issues/new?body=module:%20l10n_ch_hr_payroll%0Aversion:%2011.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
~~~~~~~

* Open Net Sàrl

Contributors
~~~~~~~~~~~~

* Sebastien Gendre <sge@open-net.ch>
* Yvon-Philippe Crittin <cyp@open-net.ch>

Maintainers
~~~~~~~~~~~

This module is maintained by the OCA.

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

This module is part of the `OCA/l10n-switzerland <https://github.com/OCA/l10n-switzerland/tree/11.0/l10n_ch_hr_payroll>`_ project on GitHub.

You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
