2.03 Changelog
^^^^^^^^^^^^^^

Changes / additions to IATI Standard for version 2.03

Note: Version 2.03 was released on Monday 19th February 2018.

.. contents::


.. _2_03_schema_changes:

Schema Changes
==============

A full diff of all schema changes in 2.03 can be found in the `IATI GitHub <https://github.com/IATI/IATI-Schemas/compare/version-2.02...version-2.03#files_bucket>`__.

These changes are also shown in the `Final Technical Summary (spreadsheet) <https://docs.google.com/spreadsheets/d/1XWnzesMvLebIVLk47OIXATfhcjESVcaGnw8SJpOuCCk/edit#gid=708614106>`__. 

Activities Schema
-----------------

- Added new @crs-channel-code attribute for the `participating-org <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/participating-org/>`__ element (`#338 <https://github.com/IATI/IATI-Schemas/issues/338>`__) (`discussion link <https://discuss.iatistandard.org/t/crs-channels-of-delivery-included-2-03/857>`__)

- Added new `tag <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/tag/>`__ element (as a child of the iati-activity element) (`#342 <https://github.com/IATI/IATI-Schemas/issues/324>`__) (`discussion link <https://discuss.iatistandard.org/t/non-statistical-secondary-sectors-excluded-2-03/849>`__)

- Updated definition: [`recipient-country <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/recipient-country/>`__, `recipient-region <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/recipient-region/>`__, `sector <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/sector/>`__] @percentage attribute (`#343 <https://github.com/IATI/IATI-Schemas/issues/343>`__) (`discussion link <https://discuss.iatistandard.org/t/boundary-values-for-percentages-included-2-03/843>`__)

- Updated definition: `sector <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/sector/>`__ @vocabulary attribute (`#344 <https://github.com/IATI/IATI-Schemas/issues/344>`__). The % sign was removed.

- Updated definition: [`transaction/aid-type <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/transaction/aid-type/>`__, `default-aid-type <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/default-aid-type/>`__] @code attribute (`#345 <https://github.com/IATI/IATI-Schemas/issues/345>`__) (`discussion link <https://discuss.iatistandard.org/t/add-vocabularies-to-aid-type-included-2-03/847>`__)

- Added new @vocabulary attributes for elements relating to `aid-type <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/transaction/aid-type/>`__ (`#346 <https://github.com/IATI/IATI-Schemas/issues/346>`__) (`discussion link <https://discuss.iatistandard.org/t/add-vocabularies-to-aid-type-included-2-03/847>`__)

- Updated definition: `capital-spend <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/capital-spend/>`__ @percentage attribute (`#348 <https://github.com/IATI/IATI-Schemas/issues/348>`__) (`discussion link <https://discuss.iatistandard.org/t/boundary-values-for-percentages-included-2-03/843>`__)

- Updated definition: `related-activity <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/related-activity/>`__ element (`#349 <https://github.com/IATI/IATI-Schemas/issues/349>`__) (`discussion link <https://discuss.iatistandard.org/t/hierarchies-related-activity-definition-included-2-03/840>`__)

- Updated occurrence: `default-aid-type <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/default-aid-type/>`__ element (`#350 <https://github.com/IATI/IATI-Schemas/issues/350>`__) (`discussion link <https://discuss.iatistandard.org/t/add-vocabularies-to-aid-type-included-2-03/847>`__)

- Updated occurrence: `transaction/aid-type <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/transaction/aid-type/>`__ element (`#351 <https://github.com/IATI/IATI-Schemas/issues/351>`__) (`discussion link <https://discuss.iatistandard.org/t/add-vocabularies-to-aid-type-included-2-03/847>`__)

Changes and Additions to the **Result** element:

- Updated definition: `result/indicator/reference <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/indicator/reference/>`__ @indicator-uri attribute (`#347 <https://github.com/IATI/IATI-Schemas/issues/347>`__) (`discussion link <https://discuss.iatistandard.org/t/guidance-on-u-r-i-usage-for-publisher-s-own-vocabularies-included-2-03/850>`__)

- Updated occurrence: `result/indicator/baseline <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/indicator/baseline/>`__ element  (`#352 <https://github.com/IATI/IATI-Schemas/issues/352>`__) (`discussion link <https://discuss.iatistandard.org/t/results-improve-consistency-of-results-standard-included-2-03/874>`__)

- Updated occurrence: `result/indicator <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/indicator/>`__ @value attributes (`#353 <https://github.com/IATI/IATI-Schemas/issues/353>`__) (`discussion link <https://discuss.iatistandard.org/t/results-represent-more-than-quantitative-data-included-2-03/872>`__)

- Updated occurrence: [`result/indicator/period/target <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/indicator/period/target/>`__, `result/indicator/period/actual <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/indicator/period/actual/>`__] elements (`#354 <https://github.com/IATI/IATI-Schemas/issues/354>`__) (`discussion link <https://discuss.iatistandard.org/t/results-allow-disaggregations-of-results-data-included-2-03/871>`__)

- Updated occurrence: `result/indicator/period/target <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/indicator/period/target/>`__ @value attribute (`#355 <https://github.com/IATI/IATI-Schemas/issues/355>`__) (`discussion link <https://discuss.iatistandard.org/t/results-represent-more-than-quantitative-data-included-2-03/872>`__)

- Updated occurrence:  `result/indicator/period/actual <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/indicator/period/actual/>`__ element (`#356 <https://github.com/IATI/IATI-Schemas/issues/356>`__) (`discussion link <https://discuss.iatistandard.org/t/results-allow-disaggregations-of-results-data-included-2-03/871>`__)

- Updated occurrence:  `result/indicator/period/actual <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/indicator/period/actual/>`__ @value attribute (`#358 <https://github.com/IATI/IATI-Schemas/issues/358>`__) (`discussion link <https://discuss.iatistandard.org/t/results-represent-more-than-quantitative-data-included-2-03/872>`__)

- Added new `document-link <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/document-link/>`__ element (as a child of various `result <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/>`__ elements)(`#359 <https://github.com/IATI/IATI-Schemas/issues/359>`__) (`discussion link <https://discuss.iatistandard.org/t/add-document-link-to-results-indicator-included-2-03/895>`__)

- Added new `reference <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/reference/>`__ element (as a child of the `result <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/>`__ element) (`#362 <https://github.com/IATI/IATI-Schemas/issues/362>`__) (`discussion link <https://discuss.iatistandard.org/t/results-vocabulary-attribute-option-included-2-03/879>`__)

- Added new @aggregation-status attribute for the `result/indicator <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/indicator/>`__ element (`#363 <https://github.com/IATI/IATI-Schemas/issues/363>`__) (`discussion link <https://discuss.iatistandard.org/t/results-improve-consistency-of-results-standard-included-2-03/874>`__)

- Added new `location <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/indicator/baseline/location/>`__ element (as a child of the `result/indicator/baseline <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/indicator/baseline/>`__ element) (`#365 <https://github.com/IATI/IATI-Schemas/issues/365>`__) (`discussion link <https://discuss.iatistandard.org/t/results-improve-consistency-of-results-standard-included-2-03/874>`__)

- Added new `dimension <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/indicator/baseline/dimension/>`__ element (as a child of the `result/indicator/baseline <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/result/indicator/baseline/>`__ element) (`#366 <https://github.com/IATI/IATI-Schemas/issues/366>`__) (`discussion link <https://discuss.iatistandard.org/t/results-allow-disaggregations-of-results-data-included-2-03/871>`__)

Organisations Schema
--------------------

- Updated definition: `organisation-identifier <http://iatistandard.org/203/organisation-standard/iati-organisations/iati-organisation/organisation-identifier/>`__ element (`#361 <https://github.com/IATI/IATI-Schemas/issues/361>`__) (`discussion link <https://discuss.iatistandard.org/t/migration-of-organisationregistrationagency-codelist-to-org-id-guide-included-2-03/851>`__)

Activities and Organisations Schemas
------------------------------------

- Updated definition: all @xml:lang attributes (`#336 <https://github.com/IATI/IATI-Schemas/issues/336>`__) (`discussion link <https://discuss.iatistandard.org/t/language-recommend-use-of-iso-639-1-included-2-03/842>`__)

- Updated definition: [`participating-org <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/participating-org/>`__, `planned-disbursement/provider-org <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/planned-disbursement/provider-org/>`__, `planned-disbursement/receiver-org <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/planned-disbursement/receiver-org/>`__, `transaction/provider-org <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/transaction/provider-org/>`__, `transaction/receiver-org <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/transaction/receiver-org/>`__, `recipient-org-budget/recipient-org <http://iatistandard.org/203/organisation-standard/iati-organisations/iati-organisation/recipient-org-budget/recipient-org/>`__] @ref attribute (`#339 <https://github.com/IATI/IATI-Schemas/issues/339>`__) (`discussion link <https://discuss.iatistandard.org/t/migration-of-organisationregistrationagency-codelist-to-org-id-guide-included-2-03/851>`__)

- Updated definition: `reporting-org <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/reporting-org/>`__ @ref attribute and `iati-organisation/organisation-identifier <http://iatistandard.org/203/organisation-standard/iati-organisations/iati-organisation/organisation-identifier/>`__ element (`#339 <https://github.com/IATI/IATI-Schemas/issues/339>`__) (`discussion link <https://discuss.iatistandard.org/t/migration-of-organisationregistrationagency-codelist-to-org-id-guide-included-2-03/851>`__)

- Updated definition: `reporting-org <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/reporting-org/>`__ @secondary-reporter attribute (`#340 <https://github.com/IATI/IATI-Schemas/issues/340>`__) (`discussion link <https://discuss.iatistandard.org/t/modify-definition-of-secondary-publisher-included-2-03/846>`__)

- Updated definition: [`recipient-region <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/recipient-region/>`__, `recipient-region-budget <http://iatistandard.org/203/organisation-standard/iati-organisations/iati-organisation/recipient-region-budget/>`__, `sector <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/sector/>`__] @vocabulary-uri attribute (`#341 <https://github.com/IATI/IATI-Schemas/issues/341>`__) (`discussion link <https://discuss.iatistandard.org/t/guidance-on-u-r-i-usage-for-publisher-s-own-vocabularies-included-2-03/850>`__)

- Added new `description <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/document-link/description/>`__ element (as a child of all `document-link <http://iatistandard.org/203/activity-standard/iati-activities/iati-activity/document-link/>`__ elements) (`#357 <https://github.com/IATI/IATI-Schemas/issues/357>`__) (`discussion link <https://discuss.iatistandard.org/t/document-link-description-included-2-03/841>`__)

.. _2_03_codelist_changes:

Codelist Changes
================

A full diff of all **embedded** codelist changes in 2.03 can be found in the `IATI GitHub <https://github.com/IATI/IATI-Codelists/compare/version-2.02...version-2.03#files_bucket>`__

Embedded to Non-Embedded:
-------------------------

Alongside 2.03, the following codelists have moved from Embedded to Non-Embedded (`#114 <https://github.com/IATI/IATI-Codelists/issues/114>`__) (`Discussion link <https://discuss.iatistandard.org/t/redefine-selected-codelists-as-non-embedded-included-2-03/854>`__):

-	`ActivityScope </en/iati-standard/203/codelists/ActivityScope>`_
-	`BudgetIdentifier </en/iati-standard/203/codelists/BudgetIdentifier>`_
-	`BudgetIdentifierSector-category </en/iati-standard/203/codelists/BudgetIdentifierSector-category>`_
-	`BudgetIdentifierSector </en/iati-standard/203/codelists/BudgetIdentifierSector>`_
-	`BudgetIdentifierVocabulary </en/iati-standard/203/codelists/BudgetIdentifierVocabulary>`_
-	`CRSAddOtherFlags </en/iati-standard/203/codelists/CRSAddOtherFlags>`_
-	`ConditionType </en/iati-standard/203/codelists/ConditionType>`_
-	`ContactType </en/iati-standard/203/codelists/ContactType>`_
-	`DescriptionType </en/iati-standard/203/codelists/DescriptionType>`_
-	`DisbursementChannel </en/iati-standard/203/codelists/DisbursementChannel>`_
-	`DocumentCategory-category </en/iati-standard/203/codelists/DocumentCategory-category>`_
-	`GeographicExactness </en/iati-standard/203/codelists/GeographicExactness>`_
-	`GeographicLocationClass </en/iati-standard/203/codelists/GeographicLocationClass>`_
-	`GeographicLocationReach </en/iati-standard/203/codelists/GeographicLocationReach>`_
-	`GeographicVocabulary </en/iati-standard/203/codelists/GeographicVocabulary>`_
-	`GeographicalPrecision </en/iati-standard/203/codelists/GeographicalPrecision>`_
-	`IndicatorMeasure </en/iati-standard/203/codelists/IndicatorMeasure>`_
-	`LoanRepaymentPeriod </en/iati-standard/203/codelists/LoanRepaymentPeriod>`_
-	`LoanRepaymentType </en/iati-standard/203/codelists/LoanRepaymentType>`_
-	`OrganisationType </en/iati-standard/203/codelists/OrganisationType>`_
-	`OtherIdentifierType </en/iati-standard/203/codelists/OtherIdentifierType>`_
-	`PolicyMarker </en/iati-standard/203/codelists/PolicyMarker>`_
-	`PolicyMarkerVocabulary </en/iati-standard/203/codelists/PolicyMarkerVocabulary>`_
-	`PublisherType </en/iati-standard/203/codelists/PublisherType>`_
-	`RegionVocabulary </en/iati-standard/203/codelists/RegionVocabulary>`_
-	`ResultType </en/iati-standard/203/codelists/ResultType>`_
-	`SectorVocabulary </en/iati-standard/203/codelists/SectorVocabulary>`_
-	`TiedStatus </en/iati-standard/203/codelists/TiedStatus>`_
-	`VerificationStatus </en/iati-standard/203/codelists/VerificationStatus>`_

New Codelists
-------------

**Non-Embedded:**

- Added `AidTypeVocabulary </en/iati-standard/203/codelists/AidTypeVocabulary>`_ Codelist (`#185 <https://github.com/IATI/IATI-Codelists-NonEmbedded/issues/185>`__) (`Discussion link <https://discuss.iatistandard.org/t/add-vocabularies-to-aid-type-included-2-03/847>`__)
- Added `BudgetNotProvided </en/iati-standard/203/codelists/BudgetNotProvided>`_ Codelist (`#184 <https://github.com/IATI/IATI-Codelists-NonEmbedded/issues/184>`__) (`Discussion link <https://discuss.iatistandard.org/t/add-budget-exempt-attribute-and-codelist-included-2-03/845>`__)
- Added `ResultVocabulary </en/iati-standard/203/codelists/ResultVocabulary>`_ Codelist (`#181 <https://github.com/IATI/IATI-Codelists/issues/181>`__) (`Discussion link <https://discuss.iatistandard.org/t/results-vocabulary-attribute-option-included-2-03/879>`__)
- Added `TagVocabulary </en/iati-standard/203/codelists/TagVocabulary>`_ Codelist (`#178 <https://github.com/IATI/IATI-Codelists-NonEmbedded/issues/178>`__) (`Discussion link <https://discuss.iatistandard.org/t/non-statistical-secondary-sectors-excluded-2-03/849>`__)

Updated Codelists
-----------------

**Embedded:**

- Added codes: 12 'Outgoing Pledge' and 13 'Incoming Pledge' to `TransactionType </en/iati-standard/203/codelists/TransactionType>`_ Codelist (`#112 <https://github.com/IATI/IATI-Codelists/issues/112>`__) (`Discussion link <https://discuss.iatistandard.org/t/transactiontype-codes-included-2-03/852>`__).

**Non-Embedded:**

- Added codes: 11 'Local Government', 24 'Partner Country based NGO', 71 'Private Sector in Provider Country', 71 'Private Sector in Aid Recipient Country', 73 'Private Sector in Third Country' and 90 'Other' to `OrganisationType </en/iati-standard/203/codelists/OrganisationType>`_ Codelist (`#113 <https://github.com/IATI/IATI-Codelists/issues/113>`__) (`Discussion link <https://discuss.iatistandard.org/t/organisation-type-codes-additions-included-2-03/858>`__)

- Added codes: 3 'Nominal', 4 'Ordinal' and 5 'Qualitative' to `IndicatorMeasure </en/iati-standard/203/codelists/IndicatorMeasure>`_ Codelist (`#179 <https://github.com/IATI/IATI-Codelists-NonEmbedded/issues/179>`__) (`Discussion link <https://discuss.iatistandard.org/t/results-represent-more-than-quantitative-data-included-2-03/872>`__)

- Added Code 2.03 to `Version </en/iati-standard/203/codelists/Version>`_ (`#238 <https://github.com/IATI/IATI-Codelists-NonEmbedded/issues/238>`__)

 .. _2_03_ruleset_changes:

Ruleset Changes
===============

A full diff of all Ruleset changes in 2.03 can be found in the `IATI GitHub <https://github.com/IATI/IATI-Codelists/compare/version-2.02...version-2.03#files_bucket>`__

- Added rule: reference element (`#48 <https://github.com/IATI/IATI-Rulesets/issues/48>`__) (`Discussion link <https://discuss.iatistandard.org/t/results-vocabulary-attribute-option-included-2-03/879>`__)

- Added rules: result @value presence - quantitative (`#51 <https://github.com/IATI/IATI-Rulesets/issues/51>`__) (`Discussion link <https://discuss.iatistandard.org/t/results-represent-more-than-quantitative-data-included-2-03/872>`__)

- Added rules: result @value presence - qualitative  (`#52 <https://github.com/IATI/IATI-Rulesets/issues/52>`__) (`Discussion link <https://discuss.iatistandard.org/t/results-represent-more-than-quantitative-data-included-2-03/872>`__)
