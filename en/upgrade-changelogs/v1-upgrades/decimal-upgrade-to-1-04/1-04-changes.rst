1.04 changes
============

Changes / Additions to IATI Standard for version 1.04

Schema Changes
--------------

A full diff of all schema changes in 1.04 can be found in github at https://github.com/IATI/IATI-Schemas/compare/version-1.03...version-1.04#files_bucket

.. _1_04_activities_schema_changes:

Activities schema
~~~~~~~~~~~~~~~~~

- Added `reporting-org/@secondary-reporter </en/iati-standard/104/activity-standard/iati-activities/iati-activity/reporting-org>`_ attribute (`discussion <http://support.iatistandard.org/entries/28509756-Add-secondary-publisher-info>`__)

- `country-budget-items/budget-item/@percentage </en/iati-standard/104/activity-standard/iati-activities/iati-activity/country-budget-items/budget-item>`_ is now optional rather than required (`discussion <http://support.iatistandard.org/entries/49964613-Bug-Fix-make-budget-item-percentage-optional>`__)

- Added `conditions/condition/@xml:lang </en/iati-standard/104/activity-standard/iati-activities/iati-activity/conditions/condition>`_ attribute. (`discussion <http://support.iatistandard.org/entries/28296716-Condition-is-missing-a-language-attribute>`__)

- Made a number of changes to the `iati-activities/iati-activity/location </en/iati-standard/104/activity-standard/iati-activities/iati-activity/location>`_ element (`discussion <http://support.iatistandard.org/entries/30343967-Summary-of-Geocoding-Changes>`__)

  * added ``location/@ref`` attribute
  * added `location/location-reach </en/iati-standard/104/activity-standard/iati-activities/iati-activity/location/location-reach>`_ element
  * added `location/location-id </en/iati-standard/104/activity-standard/iati-activities/iati-activity/location/location-id>`_ element
  * added `location/activity-description </en/iati-standard/104/activity-standard/iati-activities/iati-activity/location/activity-description>`_ element
  * `location/administrative </en/iati-standard/104/activity-standard/iati-activities/iati-activity/location/administrative>`_ gets new attributes:  ``@level``, ``@vocabulary``, ``@code``, ``@xml:lang``
  * `location/administrative </en/iati-standard/104/activity-standard/iati-activities/iati-activity/location/administrative>`_ has the following attributes deprecated: ``@country``, ``@adm1``, ``@adm2``
  * added `location/point </en/iati-standard/104/activity-standard/iati-activities/iati-activity/location/point>`_ element
  * added `location/exactness </en/iati-standard/104/activity-standard/iati-activities/iati-activity/location/exactness>`_ element
  * added `location/location-class </en/iati-standard/104/activity-standard/iati-activities/iati-activity/location/location-class>`_ element
  * added `location/feature-designation </en/iati-standard/104/activity-standard/iati-activities/iati-activity/location/feature-designation>`_ element
  * deprecated `location/gazetteer-entry </en/iati-standard/104/activity-standard/iati-activities/iati-activity/location/gazetteer-entry>`_ element
  * deprecated `location/coordinates </en/iati-standard/104/activity-standard/iati-activities/iati-activity/location/coordinates>`_ element
  * deprecated `location/location-type </en/iati-standard/104/activity-standard/iati-activities/iati-activity/location/location-type>`_ element

- Some documentation has been altered slightly

- The order that some elements are listed has changed, as this order is now used to populate the website (`commit <https://github.com/IATI/IATI-Schemas/commit/853dc481802817f1add7c7993feae5cfe08f2c06>`__)

Codelist Changes
----------------

In 1.04 the idea of Embedded and Non-Embedded codelists was introduced. See `codelist-management </en/iati-standard/104/codelists/codelist-management>`_ for more information.

A `codelist mapping file <https://github.com/IATI/IATI-Codelists/blob/version-1.04/mapping.xml>`__ describing the mapping between codelists and xml elements, was introduced. (`discussion <http://support.iatistandard.org/entries/27805388-Mapping-between-codelists-and-schemas>`__)

New Codelists
~~~~~~~~~~~~~

Embedded:

- `GeographicExactness </en/iati-standard/104/codelists/GeographicExactness>`_
- `GeographicLocationClass </en/iati-standard/104/codelists/GeographicLocationClass>`_
- `GeographicLocationReach </en/iati-standard/104/codelists/GeographicLocationReach>`_
- `GeographicVocabulary </en/iati-standard/104/codelists/GeographicVocabulary>`_

Non-Embedded:

- `OrganisationRegistrationAgency </en/iati-standard/104/codelists/OrganisationRegistrationAgency>`_ (was previously a Google Doc)

Updated Codelists
~~~~~~~~~~~~~~~~~

Embedded:

- Added ``9`` (Other) to `ResultType </en/iati-standard/104/codelists/ResultType>`_ (`discussion <http://support.iatistandard.org/entries/24090113-Suggestion-Add-other-or-undefined-to-Result-type-codelist>`__)
- Added ``NACE`` to `Vocabulary </en/iati-standard/104/codelists/Vocabulary>`_ (`discussion <http://support.iatistandard.org/entries/29678047-Add-NACE-Codes-as-a-Vocabulary-for-Sector?page=1#post_25391443>`__)
- The categories of `BudgetIdentifierSector </en/iati-standard/104/codelists/BudgetIdentifierSector>`_ have been described differently. No codes have changed.
- The "Agency Level" (``B``) category of `DocumentCategory </en/iati-standard/104/codelists/DocumentCategory>`_ has been renamed to "Organisation Level" for consistency. (`issue <https://github.com/IATI/IATI-Codelists/issues/28>`__)

Non-Embedded:

- `FileFormat </en/iati-standard/104/codelists/FileFormat>`_ updated to include all IANA Media Types. Note that it no longer has names corresponding to the codes, as the source codelist does not have this. (`discussion <http://support.iatistandard.org/entries/22915207-Additions-to-File-Format-code-list>`__)
- `LocationType </en/iati-standard/104/codelists/LocationType>`_ updated to include all US NGA Feature Designation Codes
- `Sector </en/iati-standard/104/codelists/Sector>`_ re-aligned with DAC values (`commit <https://github.com/IATI/IATI-Codelists-NonEmbedded/commit/1cf0f9baa9b0eba52d9230917cab729567fe6bc8>`__)
- `Country </en/iati-standard/104/codelists/Country>`_ adds deprecated ISO value, ``AN`` that is still in use in some IATI data (`commit <https://github.com/IATI/IATI-Codelists-NonEmbedded/commit/1cf0f9baa9b0eba52d9230917cab729567fe6bc8>`__)
