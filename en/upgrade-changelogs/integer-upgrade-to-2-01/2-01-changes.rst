2.01 Changelog
^^^^^^^^^^^^^^

Changes / additions to IATI Standard for version 2.01

Note: Version 2.01 was released on Tuesday 6 January 2015.

.. contents::

Schema Changes
==============

A full diff of all schema changes in 2.01 can be found in the `IATI GitHub <https://github.com/IATI/IATI-Schemas/compare/version-1.05...version-2.01#files_bucket>`__

Activities schema
-----------------
*Activity Website: Removed Element*
```````````````````````````````````
Element: ``activity-website`` (`discussion <http://support.iatistandard.org/entries/76684383-Redefine-activity-website-as-a-document-link>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#renamed-moved-and-removed-elements>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - activity-website
     - (removed)

*Contact Info - Department: New Element*
````````````````````````````````````````
Element: `contact-info/department </en/iati-standard/201/activity-standard/iati-activities/iati-activity/contact-info/department>`_
(`discussion <http://support.iatistandard.org/entries/44571616-Organisational-unit-within-contact-details>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#new-elements>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - (none)
     - contact-info/department

*Description: Removed Attributes*
`````````````````````````````````
* Element: `country-budget-items/budget-item/description </en/iati-standard/201/activity-standard/iati-activities/iati-activity/country-budget-items/budget-item/description>`_
* Element: `result/description </en/iati-standard/201/activity-standard/iati-activities/iati-activity/result/description/>`_
* Element: `result/indicator/description </en/iati-standard/201/activity-standard/iati-activities/iati-activity/result/indicator/description/>`_

(`discussion <http://support.iatistandard.org/entries/52106609-Version-2-01-Iteration-3-8-Miscellaneous>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#removal-of-the-type-attribute-on-some-description-elements>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - country-budget-items/budget-item/description/\@type
     - (removed)
   * - result/description/\@type
     - (removed)
   * - result/indicator/description/\@type
     - (removed)

*Document Link: Bug Fix*
````````````````````````
Inconsistencies in the document-link element were identified and applied, around the mandatory use of the language and title child elements.

* Element: `document-link </en/iati-standard/201/activity-standard/iati-activities/iati-activity/document-link>`_
(`discussion <https://github.com/IATI/IATI-Schemas/pull/256>`__ )


*Freetext: Amended Elements*
````````````````````````````
The ability to add free text has been removed from the following elements:

(`discussion <http://support.iatistandard.org/entries/41585166-General-Standardise-multi-lingual-text-fields>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#descriptive-text-is-no-longer-allowed-on-data-specified-by-codes-with-some-exceptions>`__)

* Element: `activity-status </en/iati-standard/201/activity-standard/iati-activities/iati-activity/activity-status>`_
* Element: `activity-scope </en/iati-standard/201/activity-standard/iati-activities/iati-activity/activity-scope>`_
* Element: `collaboration-type </en/iati-standard/201/activity-standard/iati-activities/iati-activity/collaboration-type>`_
* Element: `default-finance-type </en/iati-standard/201/activity-standard/iati-activities/iati-activity/default-finance-type>`_
* Element: `default-flow-type </en/iati-standard/201/activity-standard/iati-activities/iati-activity/default-flow-type>`_
* Element: `default-aid-type </en/iati-standard/201/activity-standard/iati-activities/iati-activity/default-aid-type>`_
* Element: `default-tied-status </en/iati-standard/201/activity-standard/iati-activities/iati-activity/default-tied-status>`_
* Element: `transaction/transaction-type </en/iati-standard/201/activity-standard/iati-activities/iati-activity/transaction/transaction-type>`_
* Element: `transaction/flow-type </en/iati-standard/201/activity-standard/iati-activities/iati-activity/transaction/flow-type>`_
* Element: `transaction/aid-type </en/iati-standard/201/activity-standard/iati-activities/iati-activity/transaction/aid-type>`_
* Element: `transaction/finance-type </en/iati-standard/201/activity-standard/iati-activities/iati-activity/transaction/finance-type>`_
* Element: `transaction/tied-status </en/iati-standard/201/activity-standard/iati-activities/iati-activity/transaction/tied-status>`_
* Element: `transaction/disbursement-channel </en/iati-standard/201/activity-standard/iati-activities/iati-activity/transaction/disbursement-channel>`_
* Element: `document-link/category </en/iati-standard/201/activity-standard/iati-activities/iati-activity/document-link/category>`_
* Element: `document-link/language </en/iati-standard/201/activity-standard/iati-activities/iati-activity/document-link/language>`_
* Element: `related-activity </en/iati-standard/201/activity-standard/iati-activities/iati-activity/related-activity>`_
* Element: `crs-add/loan-terms/repayment-type </en/iati-standard/201/activity-standard/iati-activities/iati-activity/crs-add/loan-terms/repayment-type>`_
* Element: `crs-add/loan-terms/repayment-plan </en/iati-standard/201/activity-standard/iati-activities/iati-activity/crs-add/loan-terms/repayment-plan>`_
* Element: `location/exactness </en/iati-standard/201/activity-standard/iati-activities/iati-activity/location/exactness>`_
* Element: `location/location-id </en/iati-standard/201/activity-standard/iati-activities/iati-activity/location/location-id>`_
* Element: `location/administrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/location/administrative>`_

*IATI Activity: Removed Attribute*
``````````````````````````````````
Element: `iati-activity </en/iati-standard/201/activity-standard/iati-activities/iati-activity/>`_ (`discussion <http://support.iatistandard.org/entries/52824355-Version-2-01-Iteration-3-9-Organisation-and-Activity-Identifiers>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#update-to-other-identifier-adding-type-changing-definition-new-codelist>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - iati-activity/\@version
     - (removed)

*Location: Removed Elements*
````````````````````````````
Element: `location </en/iati-standard/201/activity-standard/iati-activities/iati-activity/location>`_
(`discussion <http://support.iatistandard.org/entries/51310806-Delete-don-t-just-deprecate-codes-in-2-01>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#location-changes>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - location/coordinates
     - (removed)
   * - location/gazetteer-entry
     - (removed)
   * - location/location-type
     - (removed)

*Location: Removed Attributes*
``````````````````````````````
Element: `location </en/iati-standard/201/activity-standard/iati-activities/iati-activity/location>`_
(`discussion <http://support.iatistandard.org/entries/51310806-Delete-don-t-just-deprecate-codes-in-2-01>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#location-changes>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - location/\@percentage
     - (removed)
   * - location/administrative/\@country
     - (removed)
   * - location/administrative/\@adm1
     - (removed)
   * - location/administrative/\@adm2
     - (removed)

*Narrative: New Elements*
`````````````````````````
A ``narrative`` child element was added to the following elements, to enable the inclusion free text.

(`discussion <http://support.iatistandard.org/entries/41585166-General-Standardise-multi-lingual-text-fields>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#new-elements>`__)

* Element: `reporting-org/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/reporting-org/narrative>`_
* Element: `title/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/title/narrative>`_
* Element: `description/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/description/narrative>`_
* Element: `participating-org/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/participating-org/narrative>`_
* Element: `activity-date/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/activity-date/narrative>`_
* Element: `contact-info/organisation/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/contact-info/organisation/narrative>`_
* Element: `contact-info/department/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/contact-info/department/narrative>`_
* Element: `contact-info/person-name/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/contact-info/person-name/narrative>`_
* Element: `contact-info/job-title/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/contact-info/job-title/narrative>`_
* Element: `contact-info/mailing-address/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/contact-info/mailing-address/narrative>`_
* Element: `recipient-country/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/recipient-country/narrative>`_
* Element: `recipient-region/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/recipient-region/narrative>`_
* Element: `location/name/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/location/name/narrative>`_
* Element: `location/description/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/location/description/narrative>`_
* Element: `location/activity-description/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/location/activity-description/narrative>`_
* Element: `sector/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/sector/narrative>`_
* Element: `country-budget-items/budget-item/description/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/country-budget-items/budget-item/description/narrative>`_
* Element: `policy-marker/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/policy-marker/narrative>`_
* Element: `transaction/description/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/transaction/description/narrative>`_
* Element: `transaction/sector/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/transaction/sector/narrative>`_
* Element: `transaction/recipient-country/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/transaction/recipient-country/narrative>`_
* Element: `transaction/recipient-region/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/transaction/recipient-region/narrative>`_
* Element: `document-link/title/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/document-link/title/narrative>`_
* Element: `conditions/condition/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/conditions/condition/narrative>`_
* Element: `result/title/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/result/title/narrative>`_
* Element: `result/description/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/result/description/narrative>`_
* Element: `result/indicator/title/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/result/indicator/title/narrative>`_
* Element: `result/indicator/description/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/result/indicator/description/narrative>`_
* Element: `result/indicator/baseline/comment/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/result/indicator/baseline/comment/narrative>`_
* Element: `result/indicator/period/target/comment/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/result/indicator/period/target/comment/narrative>`_
* Element: `result/indicator/period/actual/comment/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/result/indicator/period/actual/comment/narrative>`_

*Other Flags: Renamed Element*
``````````````````````````````
The ``aid-type-flag`` element has been renamed to ``other-flags``.

Element: `crs-add/other-flags </en/iati-standard/201/activity-standard/iati-activities/iati-activity/crs-add/other-flags>`_
(`discussion <http://support.iatistandard.org/entries/29705458-Confusion-Between-Aid-Type-Flag-Type-of-Aid->`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#renamed-moved-and-removed-elements>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - aid-type-flag
     - other-flags

*Other Identifier: New Child Elements*
``````````````````````````````````````
The following elements were added to the ``other-identifier`` element:

(`discussion <http://support.iatistandard.org/entries/52106549-Version-2-01-Iteration-2-3-7-Replicate-more-activity-level-elements-at-transaction-level->`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#additional-elements-in-transactions-sector-recipient-country-recipient-region>`__)

* Element: `other-identifier/owner-org </en/iati-standard/201/activity-standard/iati-activities/iati-activity/other-identifier/owner-org>`_
* Element: `other-identifier/owner-org/narrative </en/iati-standard/201/activity-standard/iati-activities/iati-activity/other-identifier/owner-org/narrative>`_

*Other Identifier: Removed / New Attributes*
````````````````````````````````````````````
Element: `other-identifier </en/iati-standard/201/activity-standard/iati-activities/iati-activity/other-identifier>`_
(`discussion <http://support.iatistandard.org/entries/52824355-Version-2-01-Iteration-3-9-Organisation-and-Activity-Identifiers>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#update-to-other-identifier-adding-type-changing-definition-new-codelist>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - other-identifier/\@owner-name
     - (removed)
   * - other-identifier/\@owner-ref
     - (removed)
   * - (none)
     - other-identifier/\@ref
   * - (none)
     - other-identifier/\@type

*Planned Disbursement: Removed/Renamed Attributes*
``````````````````````````````````````````````````
Element: `planned-disbursement </en/iati-standard/201/activity-standard/iati-activities/iati-activity/planned-disbursement>`_
(`discussion <http://support.iatistandard.org/entries/77495498-Align-planned-disbursement-with-budget>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#changes-to-the-planned-disbursement-element-planned-disbursement>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - (none)
     - planned-disbursement/\@type
   * - planned-disbursement/\@last-updated
     - (removed)

*Transaction: New Child Elements*
`````````````````````````````````
The following elements were added to the ``transaction`` element:

(`discussion <http://support.iatistandard.org/entries/52106549-Version-2-01-Iteration-2-3-7-Replicate-more-activity-level-elements-at-transaction-level->`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#additional-elements-in-transactions-sector-recipient-country-recipient-region>`__)

* Element: `transaction/sector </en/iati-standard/201/activity-standard/iati-activities/iati-activity/transaction/sector>`_
* Element: `transaction/recipient-country </en/iati-standard/201/activity-standard/iati-activities/iati-activity/transaction/recipient-country>`_
* Element: `transaction/recipient-region </en/iati-standard/201/activity-standard/iati-activities/iati-activity/transaction/recipient-region>`_


Organisations schema
--------------------

*Budget Line: New Element*
``````````````````````````
A new ``budget-line`` element was added to the following elements.

(`discussion <http://support.iatistandard.org/entries/77259793-Org-Create-budget-line-element>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#new-elements>`__)

* Element: `total-budget/budget-line </en/iati-standard/201/organisation-standard/iati-organisations/iati-organisation/total-budget/budget-line>`_
* Element: `recipient-org-budget/budget-line </en/iati-standard/201/organisation-standard/iati-organisations/iati-organisation/recipient-org-budget/budget-line>`_
* Element: `recipient-country-budget/budget-line </en/iati-standard/201/organisation-standard/iati-organisations/iati-organisation/recipient-country-budget/budget-line>`_

*Document Link: Bug Fix*
````````````````````````
Inconsistencies in the document-link element were identified and applied, around the mandatory use of the language and title child elements.

* Element: `document-link </en/iati-standard/201/organisation-standard/iati-organisations/iati-organisation/document-link>`_
(`discussion <https://github.com/IATI/IATI-Schemas/pull/256>`__ )

*Document Link: New Child Element*
``````````````````````````````````
The ``recipient-country`` child element was added to the ``iati-organisation/document-link`` element:

Element: `document-link/recipient-country/narrative </en/iati-standard/201/organisation-standard/iati-organisations/iati-organisation/document-link/recipient-country/narrative>`_ (`discussion <http://support.iatistandard.org/entries/78420356-Org-Add-recipient-country-to-document-link>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#additional-elements-in-organisation-documents-document-link>`__)

*Freetext: Amended Elements*
````````````````````````````
The ability to add free text has been removed from the following element:

(`discussion <http://support.iatistandard.org/entries/41585166-General-Standardise-multi-lingual-text-fields>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#descriptive-text-is-no-longer-allowed-on-data-specified-by-codes-with-some-exceptions>`__)

* Element: `document-category </en/iati-standard/201/organisation-standard/iati-organisations/iati-organisation/document-category>`_

*IATI Identifier: Renamed Element*
``````````````````````````````````
The ``iati-organisation/iati-identifier`` element has been renamed to ``iati-organisation/organisation-identifier``.

Element: `iati-organisation/organisation-identifier </en/iati-standard/201/organisation-standard/iati-organisations/ iati-organisation/organisation-identifier>`_
(`discussion <http://support.iatistandard.org/entries/78421626-Org-Replace-iati-identifier-with-organisation>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#renamed-moved-and-removed-elements>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - iati-organisation/iati-identifier
     - iati-organisation/organisation-identifier

*Narrative: New Elements*
`````````````````````````
A ``narrative`` child element was added to the following elements, to enable the inclusion free text.

(`discussion <http://support.iatistandard.org/entries/44571616-Organisational-unit-within-contact-details>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#new-elements>`__)

* Element: `reporting-org/narrative </en/iati-standard/201/organisation-standard/iati-organisations/iati-organisation/reporting-org/narrative>`_
* Element: `name/narrative </en/iati-standard/201/organisation-standard/iati-organisations/iati-organisation/name/narrative>`_
* Element: `document-link/title/narrative </en/iati-standard/201/organisation-standard/iati-organisations/iati-organisation/document-link/title/narrative>`_
* Element: `document-link/recipient-country/narrative </en/iati-standard/201/organisation-standard/iati-organisations/iati-organisation/document-link/recipient-country/narrative>`_
* Element: `recipient-country-budget/recipient-country/narrative </en/iati-standard/201/organisation-standard/iati-organisations/iati-organisation/recipient-country-budget/recipient-country/narrative>`_
* Element: `recipient-org-budget/recipient-org/narrative </en/iati-standard/201/organisation-standard/iati-organisations/iati-organisation/recipient-org-budget/recipient-org/narrative>`_

*IATI Organisation: Removed Attribute*
``````````````````````````````````````
Element: `iati-organisation </en/iati-standard/201/organisation-standard/iati-organisations/iati-organisation/>`_ (`discussion <http://support.iatistandard.org/entries/52824355-Version-2-01-Iteration-3-9-Organisation-and-Activity-Identifiers>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#update-to-other-identifier-adding-type-changing-definition-new-codelist>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - iati-organisation/\@version
     - (removed)

Common schema
-------------
Many substantial changes were made in 2.01. Both the organisation and activity schema draw on the common schema for
common definitions of elements and types. The changes in the common schema are reflected in the sections above, so are
not given in detail here. For further information see the CHANGES.txt file that can be found with the
`schema </en/iati-standard/201/schema/>`_

XML supplementary schema
------------------------
No substantial changes were made in 2.01, aside from essential version references.

Registry record schema
----------------------
No substantial changes were made in 2.01, aside from essential version references.

Codelist Changes
================

New Codelists
-------------

*IATI Organisation Identifier: New codelist*
````````````````````````````````````````````
The *IATIOrganisationIdentifier* codelist has been created.

Codelist: `IATIOrganisationIdentifier </en/iati-standard/201/codelists/IATIOrganisationIdentifier>`_
(`discussion <http://support.iatistandard.org/entries/52824355-Version-2-01-Iteration-3-9-Organisation-and-Activity-Identifiers>`__)

*Other Identifier Type: New Codelist*
`````````````````````````````````````
Codelist: `OtherIdentifierType </en/iati-standard/201/codelists/OtherIdentifierType>`_
(`discussion <http://support.iatistandard.org/entries/52824355-Version-2-01-Iteration-3-9-Organisation-and-Activity-Identifiers>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#update-to-other-identifier-adding-type-changing-definition-new-codelist>`__)

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - A1
     - Reporting Organisation’s internal activity identifier
     - (none)
   * - A2
     - CRS Activity identifier
     - (none)
   * - A3
     - Previous Activity Identifier
     - The standard insists that once an activity has been reported to IATI its identifier MUST NOT be changed, even if the reporting organisation changes its organisation identifier. There may be exceptional circumstances in which this rule cannot be followed, in which case the previous identifier should be reported using this code.
   * - A9
     - Other Activity Identifier
     - (none)
   * - B1
     - Previous Reporting Organisation Identifier
     - (none)
   * - B9
     - Other Organisation Identifier
     - (none)

*Policy Marker Vocabulary: New codelist*
````````````````````````````````````````
The *PolicyMarkerVocabulary* has been created, split from the deleted *Vocabulary* codelist.

Codelist: `SectorVocabulary </en/iati-standard/201/codelists/PolicyMarkerVocabulary>`_
(`discussion <http://support.iatistandard.org/entries/78019646-Separate-vocabulary-codelists>`__)

*Sector Vocabulary: New codelist*
`````````````````````````````````
The *SectorVocabulary* has been created, split from the deleted *Vocabulary* codelist.

Codelist: `SectorVocabulary </en/iati-standard/201/codelists/SectorVocabulary>`_
(`discussion <http://support.iatistandard.org/entries/78019646-Separate-vocabulary-codelists>`__)

*Version: New Codelist*
```````````````````````
Codelist: `Version </en/iati-standard/201/codelists/Version>`_
(`discussion <http://support.iatistandard.org/entries/57866638-Tightening-up-on-version>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#declaring-the-version-of-the-iati-standard-being-used>`__)

.. list-table::
   :widths: 15 10 10 20
   :header-rows: 1

   * - Code
     - Name
     - Description
     - URL
   * - 1.01
     - (none)
     - (none)
     - http://iatistandard.org/101/
   * - 1.02
     - CRS Activity identifier
     - (none)
     - http://iatistandard.org/102/
   * - 1.03
     - (none)
     - (none)
     - http://iatistandard.org/103/
   * - 1.04
     - (none)
     - (none)
     - http://iatistandard.org/104/
   * - 1.05
     - (none)
     - (none)
     - http://iatistandard.org/105/
   * - 2.01
     - (none)
     - (none)
     -  http://iatistandard.org/201/


Embedded codelist updates
-------------------------

*Aid Type Flag: Renamed codelist*
`````````````````````````````````
The *AidTypeFlag* codelist has been renamed to *CRSAddOtherFlags*.

Codelist: `CRSAddOtherFlags </en/iati-standard/201/codelists/CRSAddOtherFlags>`_
(`discussion <http://support.iatistandard.org/entries/29705458-Confusion-Between-Aid-Type-Flag-Type-of-Aid->`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#renamed-moved-and-removed-elements>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - AidTypeFlag
     - CRSAddOtherFlags

*Activity Date Type: Amended codes*
```````````````````````````````````
Codelist: `ActivityDateType Type </en/iati-standard/201/codelists/ActivityDateType>`_
(`discussion <http://support.iatistandard.org/entries/41042407-Modify-code-list-activity-date-type-Language-neutral-conversion>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#language-neutral-codelists>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - start-planned
     - 1
   * - start-actual
     - 2
   * - end-planned
     - 3
   * - end-actual
     - 4

*Document Category: New codes*
``````````````````````````````
Codelist: `DocumentCategory </en/iati-standard/201/codelists/DocumentCategory>`_
(`discussion <http://support.iatistandard.org/entries/76684383-Redefine-activity-website-as-a-document-link>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/l#new-codes-for-embedded-codelists>`__)

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - A12
     - Activity web page
     - (none)
   * - B16
     - Organisation web page
     - (none)
   * - B17
     - Country/Region web page
     - (none)
   * - B18
     - Sector web page
     - (none)

*Gazetteer Agency: Amended codes*
`````````````````````````````````
Codelist: `GazetteerAgency </en/iati-standard/201/codelists/GazetteerAgency>`_
(`discussion <http://support.iatistandard.org/entries/41042407-Modify-code-list-activity-date-type-Language-neutral-conversion>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#language-neutral-codelists>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - GEO
     - 1
   * - NGA
     - 2
   * - OSM
     - 3

*Organisation Role: Amended codes*
``````````````````````````````````
Codelist: `OrganisationRole </en/iati-standard/201/codelists/OrganisationRole>`_
(`discussion <http://support.iatistandard.org/entries/41042407-Modify-code-list-activity-date-type-Language-neutral-conversion>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#language-neutral-codelists>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - Funding
     - 1
   * - Accountable
     - 2
   * - Extending
     - 3
   * - Implementing
     - 4

*Policy Marker Vocabulary (was Vocabulary): Amended codes*
``````````````````````````````````````````````````````````
Codelist: `PolicyMarkerVocabulary </en/iati-standard/201/codelists/PolicyMarkerVocabulary>`_
(`discussion <http://support.iatistandard.org/entries/41042407-Modify-code-list-activity-date-type-Language-neutral-conversion>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#language-neutral-codelists>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - DAC
     - 1
   * - RO
     - 99

*Related Activity Type: New code*
`````````````````````````````````
Codelist: `RelatedActivityType </en/iati-standard/201/codelists/RelatedActivityType>`_
(`discussion <http://support.iatistandard.org/entries/76684383-Redefine-activity-website-as-a-document-link>`__ | `guidance <http://support.iatistandard.org/entries/76862583-Referencing-another-publisher-s-report-of-the-same-activity>`__)

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - 5
     - Third Party
     - A report by another organisation on the same activity (excluding activities reported as part of financial transactions - eg. provider-activity-id - or a co-funded activity using code = 4)


*Sector Vocabulary (was Vocabulary): Amended codes*
```````````````````````````````````````````````````
Codelist: `SectorVocabulary </en/iati-standard/201/codelists/SectorVocabulary>`_
(`discussion <http://support.iatistandard.org/entries/41042407-Modify-code-list-activity-date-type-Language-neutral-conversion>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#language-neutral-codelists>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - ADT
     - 1
   * - COFOG
     - 2
   * - DAC
     - 3
   * - DAC-3
     - 4
   * - ISO
     - 5
   * - NACE
     - 6
   * - NTEE
     - 7
   * - WB
     - 8
   * - RO
     - 99

*Transaction Type: Amended codes*
`````````````````````````````````
Codelist: `TransactionType </en/iati-standard/201/codelists/TransactionType>`_
(`discussion <http://support.iatistandard.org/entries/41042407-Modify-code-list-activity-date-type-Language-neutral-conversion>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#language-neutral-codelists>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - IF
     - 1
   * - C
     - 2
   * - D
     - 3
   * - E
     - 4
   * - IR
     - 5
   * - LR
     - 6
   * - R
     - 7
   * - QP
     - 8
   * - Q3
     - 9
   * - CG
     - 10

*Vocabulary: Removed / split codelist*
``````````````````````````````````````
The *Vocabulary* has been removed, and split into two new codelists: *SectorVocabulary* and *PolicyMarkerVocabulary*.

Codelist: `SectorVocabulary </en/iati-standard/201/codelists/SectorVocabulary>`_ | `SectorVocabulary </en/iati-standard/203/codelists/PolicyMarkerVocabulary>`_
(`discussion <http://support.iatistandard.org/entries/78019646-Separate-vocabulary-codelists>`__)
