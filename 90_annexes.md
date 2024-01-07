---
output: html_document
---

# (APPENDIX) ANNEXES {-}

# Annex 1: References and links {-}

**Documents**

- Asian Development Bank (ADB). 2001. [*Mapping the Spatial Distribution of Poverty Using Satellite Imagery in Thailand*](http://dx.doi.org/10.22617/TCS210112-2) ISBN 978-92-9262-768-3 (print), 978-92-9262-769-0 (electronic), 978-92-9262-770-6 (ebook)
Publication Stock No. TCS210112-2. DOI: http://dx.doi.org/10.22617/TCS210112-2

- Balashankar, A., L.Subramanian, and S.P. Fraiberger. 2021. [*Fine-grained prediction of food insecurity using news streams*](https://arxiv.org/pdf/2111.15602.pdf)

- British Ecological Society. 2017. [*Guide to Reproducible Code in Ecology and Evolution*](https://www.britishecologicalsociety.org/wp-content/uploads/2017/12/guide-to-reproducible-code.pdf) 

- Google. [Google's Search Engine Optimization (SEO) Starter Guide](https://developers.google.com/search/docs/beginner/seo-starter-guide)

- Jurafsky, Daniel; H. James, Martin. 2000. *Speech and language processing : an introduction to natural language processing, computational linguistics, and speech recognition*. Upper Saddle River, N.J.: Prentice Hall. ISBN 978-0-13-095069-7

- Mikolov, T., K.Chen, G.Corrado, and J.Dean. 2013. [*Efficient Estimation of Word Representations in Vector Space*](https://arxiv.org/abs/1301.3781)

- Min, B. and Z.O'Keeffe. 2021. http://www-personal.umich.edu/~brianmin/HREA/index.html

- Priest, G.. 2010. [*The Struggle for Integration and Harmonization of Social Statistics in a Statistical Agency - A Case Study of Statistics Canada*](https://www.ihsn.org/sites/default/files/resources/IHSN-WP004.pdf) 

- Stodden et al. 2013. [*Setting the Default to Reproducible - Reproducibility in Computational and Experimental Mathematics*](http://stodden.net/icerm_report.pdf)

- Turnbull, D. and J. Berryman. 2016. [*Relevant Search: With applications for Solr and Elasticsearch*](https://www.manning.com/books/relevant-search) 


**Links (standards, schemas, controlled vocabularies)**

- American Psychological Association (APA): [APA Style (example of specific publications styles for a table)](https://apastyle.apa.org/style-grammar-guidelines/tables-figures/tables)

- [Consortium of European Social Science Data Archives (CESSDA)](https://www.cessda.eu/)

- US Census Bureau, CsPro Users Guide: [Parts of a Table](https://www.csprousers.org/help/CSPro/parts_of_a_table.html)

- [Data Documentation Initiative (DDI) Alliance](https://ddialliance.org/)

- DDI Alliance, [Data Documentation Initiative (DDI) Codebook](https://ddialliance.org/Specification/DDI-Codebook/2.5/)

- [Dublin Core Metadata Initiative (DCMI)](https://www.dublincore.org/)

- eMathZone: [Construction of a Statistical Table](https://www.emathzone.com/tutorials/basic-statistics/construction-of-statistical-table.html)

- GoFair [(Findable, Accessible, Interoperable and Reusable (FAIR))](https://www.go-fair.org/)

- [International Household Survey Network (IHSN)](https://www.ihsn.org/)

- [International Press Telecommunications Council (IPTC)](https://iptc.org/)

- International Organization for Standardization (ISO) 19139: [Geographic information — Metadata — XML schema implementation](https://www.iso.org/standard/32557.html)

- [LabWrite: Designing Tables](https://labwrite.ncsu.edu/res/gh/gh-tables.html)

- [schema.org](https://schema.org/)

- Microsoft Bing: [Bing Webmaster Tools Help & How-To Center, Bing Webmaster Guidelines](https://www.bing.com/webmasters/help/webmaster-guidelines-30fba23a)

- [Vedantu: Tabulation](https://www.vedantu.com/commerce/tabulation)


**Links (tools)**

- [CKAN open-source data management system](https://ckan.org/)
- [ElasticSearch](https://github.com/elastic/elasticsearch) 
- [GeoNetwork](https://geonetwork-opensource.org/)
- [Milvus](https://milvus.io/))
- [NADA cataloguing application, web page](https://nada.ihsn.org/)
- [NADA cataloguing application, demo page](https://nada-demo.ihsn.org/index.php/home)
- [NADA cataloguing application, GitHub repository](https://github.com/ihsn/nada/releases/tag/V5.0.3)
- [NADAR package]()
- [Nesstar Publisher (DDI 1.n Metadata Editor](http://www.nesstar.com/)
- [R: The R Project for Statistical Computing](https://www.r-project.org/)
- [R Bookdown](https://bookdown.org/): Write HTML, PDF, ePub, and Kindle books with R Markdown
- [R geometa](https://cran.r-project.org/web/packages/geometa/index.html): Tools for Reading and Writing ISO/OGC Geographic Metadata
- [Solr](https://solr.apache.org/)

**Links (others)**

- WorldPop: https://www.worldpop.org/


# Annex 2: Mapping standards and schemas to schema.org {-}

The use of *structured data* described in section 1.6.2 requires a mapping between the relevant elements of some of the metadata standards and schemas described in the Guide to the schema.org standard. We provide here a suggested selection and mapping for the core set of elements (we do not attempt to map all possible elements that are common to our schemas and schema.org).

### Microdata

|schema.org/dataset     |DDI CodeBook     | Recommendation  |
|-----------------------|-----------------|-----------------|
|name                   |    |
|description            |    |
|url                    |    |
|sameAs                 |    |
|identifier             |    |
|keywords               |    |
|license                |    |
|isAccessibleForFree    |    |
|hasPart / isPartOf     |    |
|creator type / url  / name / contactPoint / funder |    |
|includedInDataCatalog  |    |
|distribution           |    |
|temporalCoverage       |    |
|spatialCoverage        |    |


**Example:**

```html
<html>
  <head>
    <script type="application/ld+json">
    {
      "@context":"https://schema.org/",
      "@type":"Dataset",
      "name":"Albania Living Standards Measurement Survey 2012 (LSMS 2010)",
      "description":"The Living Standards Measurement Survey (LSMS) is a multi-purpose household survey conducted to measure living conditions and poverty situation,                        and to help policymakers in monitoring and developing social programs. LSMS has been carried out in Albania in the context of continuing                                monitoring of poverty and the creation of policy evaluation system in the framework of the National Strategy for Development and Integration                            (previously the National Strategy for Economic and Social Development). The first Albania LSMS was conducted in 2002, followed by 2003, 2004,                          2005, 2008 and 2012 surveys. In 2012, 6,671 households participated in the survey.",
      "url":"https://microdata.worldbank.org/index.php/catalog/1970",
      "identifier": ["ALB_2012_LSMS_v01_M_v01_A_PUF"],
      "keywords":[
         "demographic characteristics",
         "education",
         "communication",
         "labor",
         "employment",
         "non-farm business",
         "migration",
         "remittances",
         "subjective poverty",
         "health",
         "fertility",
         "non-food expenditures",
         "dwelling",
         "utilities",
         "durable goods",
         "daily food consumption"
      ],
      "license" : "",
      "isAccessibleForFree" : true,
      "creator":[
         {
            "@type":"Organization",
            "url": "http://www.instat.gov.al/en/",
            "name":"Institute of Statistics of Albania",
            "contactPoint":{
               "@type":"ContactPoint",
               "email":"info@instat.gov.al"
         },
         { 
            "@type":"Organization",
            "url": "https://www.worldbank.org/",
            "name":"World Bank",
            "contactPoint":{
               "@type":"ContactPoint",
               "contactType": "LSMS technical support",
               "email":"lsms@worldbank.org"
            }
      ],
      "funder":{
         "@type": "Organization",
         "name": "World Bank"
      },
      "includedInDataCatalog":{
         "@type":"World Bank Microdata Library",
         "name":"https://microdata.worldbank.org/index.php/home"
      },
      "distribution":[
         {
            "@type":"DataDownload",
            "encodingFormat":"SPSS Windows (.sav)",
            "contentUrl":"http://www.instat.gov.al/en/figures/micro-data/"
         }
      ],
      "temporalCoverage":"2012",
      "spatialCoverage":{
         "@type":"Place",
         "name": "Albania"
         }
      }
    }
    </script>
  </head>
  <body>
  </body>
</html>
```

### Geographic data

|schema.org/dataset     |ISO 19139        | Recommendation  |
|-----------------------|-----------------|-----------------|
|name                   |    |
|description            |    |
|url                    |    |
|sameAs                 |    |
|identifier             |    |
|keywords               |    |
|license                |    |
|isAccessibleForFree    |    |
|hasPart / isPartOf     |    |
|creator type / url  / name / contactPoint / funder |    |
|includedInDataCatalog  |    |
|distribution           |    |
|temporalCoverage       |    |
|spatialCoverage        |    |


**Example:**



### Indicators (and database)

|schema.org/dataset     |INDICATOR schema | Recommendation  |
|-----------------------|-----------------|-----------------|
|name                   |    |
|description            |    |
|url                    |    |
|sameAs                 |    |
|identifier             |    |
|keywords               |    |
|license                |    |
|isAccessibleForFree    |    |
|hasPart / isPartOf     |    |
|creator type / url  / name / contactPoint / funder |    |
|includedInDataCatalog  |    |
|distribution           |    |
|temporalCoverage       |    |
|spatialCoverage        |    | 


**Example:**

### Tables

|schema.org/dataset     |TABLES schema    | Recommendation  |
|-----------------------|-----------------|-----------------|
|name                   |    |
|description            |    |
|url                    |    |
|sameAs                 |    |
|identifier             |    |
|keywords               |    |
|license                |    |
|isAccessibleForFree    |    |
|hasPart / isPartOf     |    |
|creator type / url  / name / contactPoint / funder |    |
|includedInDataCatalog  |    |
|distribution           |    |
|temporalCoverage       |    |
|spatialCoverage        |    |


**Example:**

### Images

The complete list of elements available in schema.org to document an image object is available at https://schema.org/ImageObject. We only show in the table below a selection of the ones we consder the most relevant and frequently available. Images can be documented either using the IPTC-based schema, or the Dublin Core (DCMI)-based schema.

|schema.org/dataset     |IMAGE schema (IPTC) | Recommendation  |
|-----------------------|--------------------|-----------------|
| name                  |  |
| abstract              |  |
| creator               |  |
| provider              |  |
| sourceOrganization    |  |
| dateCreated           |  |
| keywords              |  |
| contentLocation       |  |
| contentReferenceTime  |  |
| copyrightHolder       |  |
| copyrightNotice       |  |
| copyrightYear         |  |
| creditText            |  |
| isAccessibleForFree   |  |
| license               |  | 
| acquireLicensePage    |  |
| contentUrl            |  |


|schema.org/dataset     |IMAGE schema (DCMI) | Recommendation  |
|-----------------------|--------------------|-----------------|
| name                  |  |
| abstract              |  |
| creator               |  |
| provider              |  |
| sourceOrganization    |  |
| dateCreated           |  |
| keywords              |  |
| contentLocation       |  |
| contentReferenceTime  |  |
| copyrightHolder       |  |
| copyrightNotice       |  |
| copyrightYear         |  |
| creditText            |  |
| isAccessibleForFree   |  |
| license               |  | 
| acquireLicensePage    |  |
| contentUrl            |  |


**Example:**

<html>
  <head>
    <title>Residents get water from an artesian well, Sindh, Pakistan</title>
    <script type="application/ld+json">
    {
      "@context": "https://schema.org/",
      "@type": "ImageObject",
      "contentUrl": "https://nada-demo.ihsn.org/index.php/catalog/13",
      "license": "Attribution License",
      "acquireLicensePage": "https://nada-demo.ihsn.org/index.php/catalog/13/related-materials",
      "creditText": "",
      "creator": {
        "@type": "Person",
        "name": "Caroline Suzman"
       },
      "copyrightNotice": ""
    }
    </script>
  </head>
</html>



# Annex 3: Mapping the microdata schema to the DDI Codebook 2.5  {-}

|JSON Schema                                                           |DDI/XML CodeBook 2.5                                                        |Title                                                                  |
|----------------------------------------------------------------------|----------------------------------------------------------------------------|-----------------------------------------------------------------------|
|doc_desc                                                              |docDscr                                                                     |                                                                       |
|doc_desc/title                                                        |docDscr/citation/titlStmt/titl                                              |Document title                                                         |
|doc_desc/idno                                                         |docDscr/citation/titlStmt/IDNo                                              |Unique ID number for the document                                      |
|doc_desc/producers                                                    |docDscr/citation/prodStmt/producer                                          |Producers                                                              |
|- name                                                                |.                                                                           |Name                                                                   |
|- abbr                                                                |- abbr                                                                      |Abbreviation                                                           |
|- affiliation                                                         |- affiliation                                                               |Affiliation                                                            |
|- role                                                                |- role                                                                      |Role                                                                   |
|doc_desc/prod_date                                                    |docDscr/citation/prodStmt/prodDate                                          |Date of Production                                                     |
|doc_desc/version_statement                                            |docDscr/citation/verStmt                                                    |Version Statement                                                      |
|doc_desc/version_statement/version                                    |docDscr/citation/verStmt/version                                            |Version                                                                |
|doc_desc/version_statement/version_date                               |docDscr/citation/verStmt/version/@date                                      |Version Date                                                           |
|doc_desc/version_statement/version_resp                               |docDscr/citation/verStmt/verResp                                            |Version Responsibility Statement                                       |
|doc_desc/version_statement/version_notes                              |docDscr/citation/verStmt/notes                                              |Version Notes                                                          |
|study_desc                                                            |stdyDscr                                                                    |                                                                       |
|study_desc/title_statement                                            |stdyDscr/citation/titlStmt                                                  |                                                                       |
|study_desc/title_statement/idno                                       |stdyDscr/citation/titlStmt/IDNo                                             |Unique user defined ID                                                 |
|study_desc/title_statement/identifiers                                |                                                                            |Other identifiers                                                      |
|- type                                                                |                                                                            |Identifier type                                                        |
|- identifier                                                          |                                                                            |Identifier                                                             |
|study_desc/title_statement/title                                      |stdyDscr/citation/titlStmt/titl                                             |Survey title                                                           |
|study_desc/title_statement/sub_title                                  |stdyDscr/citation/titlStmt/subTitl                                          |Survey subtitle                                                        |
|study_desc/title_statement/alternate_title                            |stdyDscr/citation/titlStmt/altTitl                                          |Abbreviation or Acronym                                                |
|study_desc/title_statement/translated_title                           |stdyDscr/citation/titlStmt/parTitl                                          |Translated Title                                                       |
|study_desc/authoring_entity                                           |stdyDscr/citation/rspStmt/AuthEnty                                          |Authoring entity/Primary investigators                                 |
|- name                                                                |.                                                                           |Agency Name                                                            |
|- affiliation                                                         |- affiliation                                                               |Affiliation                                                            |
|study_desc/oth_id                                                     |stdyDscr/citation/rspStmt/othId                                             |Other Identifications/Acknowledgments                                  |
|- name                                                                |.                                                                           |Name                                                                   |
|- role                                                                |- role                                                                      |Role                                                                   |
|- affiliation                                                         |- affiliation                                                               |Affiliation                                                            |
|study_desc/production_statement                                       |stdyDscr/citation/prodStmt                                                  |Production Statement                                                   |
|study_desc/production_statement/producers                             |stdyDscr/citation/prodStmt/producer                                         |Producers                                                              |
|- name                                                                |.                                                                           |Name                                                                   |
|- abbr                                                                |- abbr                                                                      |Abbreviation                                                           |
|- affiliation                                                         |- affiliation                                                               |Affiliation                                                            |
|- role                                                                |- role                                                                      |Role                                                                   |
|study_desc/production_statement/copyright                             |stdyDscr/citation/prodStmt/copyright                                        |Copyright                                                              |
|study_desc/production_statement/prod_date                             |stdyDscr/citation/prodStmt/prodDate                                         |Production Date                                                        |
|study_desc/production_statement/prod_place                            |stdyDscr/citation/prodStmt/prodPlac                                         |Production Place                                                       |
|study_desc/production_statement/funding_agencies                      |stdyDscr/citation/prodStmt/fundAg                                           |Funding Agency/Sponsor                                                 |
|- name                                                                |.                                                                           |Funding Agency/Sponsor                                                 |
|- abbr                                                                |- abbr                                                                      |Abbreviation                                                           |
|- grant                                                               |- stdyDscr/citation/prodStmt/fundAg                                         |Grant Number                                                           |
|- role                                                                |- role                                                                      |Role                                                                   |
|study_desc/distribution_statement                                     |stdyDscr/citation/distStmt                                                  |Distribution Statement                                                 |
|study_desc/distribution_statement/distributors                        |stdyDscr/citation/distStmt/distrbtr                                         |Distributor                                                            |
|- name                                                                |.                                                                           |Organization name                                                      |
|- abbr                                                                |- abbr                                                                      |Abbreviation                                                           |
|- affiliation                                                         |- affiliation                                                               |Affiliation                                                            |
|- uri                                                                 |- uri                                                                       |URI                                                                    |
|study_desc/distribution_statement/contact                             |stdyDscr/citation/distStmt/contact                                          |Contact                                                                |
|- name                                                                |.                                                                           |Name                                                                   |
|- affiliation                                                         |- affiliation                                                               |Affiliation                                                            |
|- email                                                               |- email                                                                     |Email                                                                  |
|- uri                                                                 |- uri                                                                       |URI                                                                    |
|study_desc/distribution_statement/depositor                           |stdyDscr/citation/distStmt/depositr                                         |Depositor                                                              |
|- name                                                                |.                                                                           |Name                                                                   |
|- abbr                                                                |- abbr                                                                      |Abbreviation                                                           |
|- affiliation                                                         |- affiliation                                                               |Affiliation                                                            |
|- uri                                                                 |                                                                            |URI                                                                    |
|study_desc/distribution_statement/deposit_date                        |stdyDscr/citation/distStmt/depDate                                          |Date of Deposit                                                        |
|study_desc/distribution_statement/distribution_date                   |stdyDscr/citation/distStmt/distDate                                         |Date of Distribution                                                   |
|study_desc/series_statement                                           |stdyDscr/citation/serStmt                                                   |Series Statement                                                       |
|study_desc/series_statement/series_name                               |stdyDscr/citation/serStmt/serName                                           |Series Name                                                            |
|study_desc/series_statement/series_info                               |stdyDscr/citation/serStmt/serInfo                                           |Series Information                                                     |
|study_desc/version_statement                                          |stdyDscr/citation/verStmt                                                   |Version Statement                                                      |
|study_desc/version_statement/version                                  |stdyDscr/citation/verStmt/version                                           |Version                                                                |
|study_desc/version_statement/version_date                             |stdyDscr/citation/verStmt/version/@date                                     |Version Date                                                           |
|study_desc/version_statement/version_resp                             |stdyDscr/citation/verStmt/verResp                                           |Version Responsibility Statement                                       |
|study_desc/version_statement/version_notes                            |stdyDscr/citation/verStmt/notes                                             |Version Notes                                                          |
|study_desc/bib_citation                                               |stdyDscr/citation/biblCit                                                   |Bibliographic Citation                                                 |
|study_desc/bib_citation_format                                        |stdyDscr/citation/biblCit/@format                                           |Bibliographic Citation Format                                          |
|study_desc/holdings                                                   |stdyDscr/citation/holdings                                                  |Holdings Information                                                   |
|- name                                                                |.                                                                           |Name                                                                   |
|- location                                                            |- location                                                                  |Location                                                               |
|- callno                                                              |- callno                                                                    |Callno                                                                 |
|- uri                                                                 |- uri                                                                       |URI                                                                    |
|study_desc/study_notes                                                |stdyDscr/citation/notes                                                     |Study notes                                                            |
|study_desc/study_authorization                                        |stdyDscr/studyAuthorization                                                 |Study Authorization                                                    |
|study_desc/study_authorization/date                                   |stdyDscr/studyAuthorization/@date                                           |Authorization Date                                                     |
|study_desc/study_authorization/agency                                 |stdyDscr/studyAuthorization/authorizingAgency                               |Authorizing Agency                                                     |
|- name                                                                |.                                                                           |Funding Agency/Sponsor                                                 |
|- affiliation                                                         |- affiliation                                                               |Affiliation                                                            |
|- abbr                                                                |- abbr                                                                      |Abbreviation                                                           |
|study_desc/study_authorization/authorization_statement                |stdyDscr/studyAuthorization/authorizationStatement                          |Authorization Statement                                                |
|study_desc/study_info                                                 |stdyDscr/stdyInfo                                                           |Study Scope                                                            |
|study_desc/study_info/study_budget                                    |stdyDscr/stdyInfo/studyBudget                                               |Study Budget                                                           |
|study_desc/study_info/keywords                                        |stdyDscr/stdyInfo/subject/keyword                                           |                                                                       |
|- keyword                                                             |.                                                                           |Keyword                                                                |
|- vocab                                                               |- vocab                                                                     |Vocabulary                                                             |
|- uri                                                                 |- vocabURI                                                                  |uri                                                                    |
|study_desc/study_info/topics                                          |stdyDscr/stdyInfo/subject/topcClas                                          |Topic Classification                                                   |
|- topic                                                               |.                                                                           |Topic                                                                  |
|- vocab                                                               |- vocab                                                                     |Vocab                                                                  |
|- uri                                                                 |- vocabURI                                                                  |URI                                                                    |
|study_desc/study_info/abstract                                        |stdyDscr/stdyInfo/abstract                                                  |Abstract                                                               |
|study_desc/study_info/time_periods                                    |stdyDscr/stdyInfo/sumDscr/timePrd                                           |Time periods (YYYY/MM/DD)                                              |
|- start                                                               |                                                                            |Start date                                                             |
|- end                                                                 |                                                                            |End date                                                               |
|- cycle                                                               |                                                                            |Cycle                                                                  |
|study_desc/study_info/coll_dates                                      |stdyDscr/stdyInfo/sumDscr/collDate                                          |Dates of Data Collection (YYYY/MM/DD)                                  |
|- start                                                               |                                                                            |Start date                                                             |
|- end                                                                 |                                                                            |End date                                                               |
|- cycle                                                               |                                                                            |Cycle                                                                  |
|study_desc/study_info/nation                                          |stdyDscr/stdyInfo/sumDscr/nation                                            |Country                                                                |
|- name                                                                |.                                                                           |Name                                                                   |
|- abbreviation                                                        |- abbr                                                                      |Country code                                                           |
|study_desc/study_info/bbox                                            |stdyDscr/sumDscr/geoBndBox                                                  |Geographic bounding box                                                |
|- west                                                                |- westBL                                                                    |West                                                                   |
|- east                                                                |- eastBL                                                                    |East                                                                   |
|- south                                                               |- southBL                                                                   |South                                                                  |
|- north                                                               |- northBL                                                                   |North                                                                  |
|study_desc/study_info/bound_poly                                      |stdyDscr/sumDscr/boundPoly/polygon/point                                    |Geographic Bounding Polygon                                            |
|- lat                                                                 |gringLat                                                                    |Latitude                                                               |
|- lon                                                                 |gringLon                                                                    |longitude                                                              |
|study_desc/study_info/geog_coverage                                   |stdyDscr/stdyInfo/sumDscr/geogCover                                         |Geographic Coverage                                                    |
|study_desc/study_info/geog_coverage_notes                             |stdyDscr/sumDscr/geogCover/txt                                              |Geographic Coverage notes                                              |
|study_desc/study_info/geog_unit                                       |stdyDscr/stdyInfo/sumDscr/geogUnit                                          |Geographic Unit                                                        |
|study_desc/study_info/analysis_unit                                   |stdyDscr/stdyInfo/sumDscr/anlyUnit                                          |Unit of Analysis                                                       |
|study_desc/study_info/universe                                        |stdyDscr/stdyInfo/sumDscr/universe                                          |Universe                                                               |
|study_desc/study_info/data_kind                                       |stdyDscr/stdyInfo/sumDscr/dataKind                                          |Kind of Data                                                           |
|study_desc/study_info/notes                                           |stdyDscr/stdyInfo/notes                                                     |Study notes                                                            |
|study_desc/study_info/quality_statement                               |stdyDscr/stdyInfo/qualityStatement                                          |Quality Statement                                                      |
|study_desc/study_info/quality_statement/compliance_description        |stdyDscr/stdyInfo/qualityStatement/standardsCompliance/complianceDescription|Standard compliance description                                        |
|study_desc/study_info/quality_statement/standards                     |stdyDscr/stdyInfo/qualityStatement/standardsCompliance/standard             |Standards                                                              |
|- name                                                                |standardName                                                                |Name                                                                   |
|- producer                                                            |producer *                                                                  |Producer                                                               |
|study_desc/study_info/quality_statement/other_quality_statement       |stdyDscr/stdyInfo/qualityStatement/otherQualityStatement                    |Other quality statement                                                |
|study_desc/study_info/ex_post_evaluation                              |stdyDscr/stdyInfo/exPostEvaluation                                          |Ex-Post Evaluation                                                     |
|study_desc/study_info/ex_post_evaluation/completion_date              |stdyDscr/stdyInfo/exPostEvaluation/@completionDate                          |Evaluation completion date                                             |
|study_desc/study_info/ex_post_evaluation/type                         |stdyDscr/stdyInfo/@type                                                     |Evaluation type                                                        |
|study_desc/study_info/ex_post_evaluation/evaluator                    |stdyDscr/stdyInfo/exPostEvaluation/evaluator                                |Evaluators                                                             |
|- name                                                                |.                                                                           |Funding Agency/Sponsor                                                 |
|- affiliation                                                         |- affiliation                                                               |Affiliation                                                            |
|- abbr                                                                |- abbr                                                                      |Abbreviation                                                           |
|- role                                                                |- role                                                                      |Role                                                                   |
|study_desc/study_info/ex_post_evaluation/evaluation_process           |stdyDscr/stdyInfo/exPostEvaluation/evaluationProcess                        |Evaluation process                                                     |
|study_desc/study_info/ex_post_evaluation/outcomes                     |stdyDscr/stdyInfo/exPostEvaluation/outcomes                                 |Outcomes                                                               |
|study_desc/study_development                                          |stdyDscr/studyDevelopment                                                   |Study Development                                                      |
|study_desc/study_development/development_activity                     |stdyDscr/studyDevelopment/developmentActivity                               |Development activity                                                   |
|- activity_type                                                       |.                                                                           |Development activity type                                              |
|- activity_description                                                |- description                                                               |Development activity description                                       |
|- participants                                                        |- participants                                                              |Participants                                                           |
|- resources                                                           |- resources                                                                 |Development activity resources                                         |
|- outcome                                                             |- outcome                                                                   |Development Activity Outcome                                           |
|study_desc/method                                                     |stdyDscr/method                                                             |Methodology and Processing                                             |
|study_desc/method/data_collection                                     |stdyDscr/method/dataColl                                                    |Data Collection                                                        |
|study_desc/method/data_collection/time_method                         |stdyDscr/method/dataColl/timeMeth                                           |Time Method                                                            |
|study_desc/method/data_collection/data_collectors                     |stdyDscr/method/dataColl/dataCollector                                      |Data Collectors                                                        |
|- name                                                                |.                                                                           |Name                                                                   |
|- affiliation                                                         |                                                                            |Affiliation                                                            |
|- abbr                                                                |                                                                            |Abbreviation                                                           |
|- role                                                                |                                                                            |Role                                                                   |
|study_desc/method/data_collection/collector_training                  |stdyDscr/method/dataColl/collectorTraining                                  |Collector training                                                     |
|- type                                                                |@type                                                                       |Training type                                                          |
|- training                                                            |.                                                                           |Training                                                               |
|study_desc/method/data_collection/frequency                           |stdyDscr/method/dataColl/frequenc                                           |Frequency of Data Collection                                           |
|study_desc/method/data_collection/sampling_procedure                  |stdyDscr/method/dataColl/sampProc                                           |Sampling Procedure                                                     |
|study_desc/method/data_collection/sample_frame                        |stdyDscr/method/dataColl/sampleFrame                                        |Sample Frame                                                           |
|study_desc/method/data_collection/sample_frame/name                   |stdyDscr/method/dataColl/sampleFrame/sampleFrameName                        |Sample frame name                                                      |
|study_desc/method/data_collection/sample_frame/valid_period           |stdyDscr/method/dataColl/sampleFrame/validPeriod                            |Valid periods (YYYY/MM/DD)                                             |
|- event                                                               |                                                                            |Event                                                                  |
|- date                                                                |                                                                            |Date                                                                   |
|study_desc/method/data_collection/sample_frame/custodian              |stdyDscr/method/dataColl/sampleFrame/custodian                              |Custodian                                                              |
|study_desc/method/data_collection/sample_frame/universe               |stdyDscr/method/dataColl/sampleFrame/universe                               |Universe                                                               |
|study_desc/method/data_collection/sample_frame/frame_unit             |stdyDscr/method/dataColl/sampleFrame/frameUnit                              |Frame unit                                                             |
|study_desc/method/data_collection/sample_frame/frame_unit/is_primary  |stdyDscr/method/dataColl/sampleFrame/frameUnit/@isPrimary                   |Is Primary                                                             |
|study_desc/method/data_collection/sample_frame/frame_unit/unit_type   |stdyDscr/method/dataColl/sampleFrame/frameUnit/unitType                     |Unit Type                                                              |
|study_desc/method/data_collection/sample_frame/frame_unit/num_of_units|stdyDscr/method/dataColl/sampleFrame/frameUnit/@numberOfUnits               |Number of units                                                        |
|study_desc/method/data_collection/sample_frame/reference_period       |stdyDscr/method/dataColl/sampleFrame/referencePeriod                        |Reference periods (YYYY/MM/DD)                                         |
|- event                                                               |                                                                            |Event                                                                  |
|- date                                                                |                                                                            |Date                                                                   |
|study_desc/method/data_collection/sample_frame/update_procedure       |stdyDscr/method/dataColl/sampleFrame/updateProcedure                        |Update procedure                                                       |
|study_desc/method/data_collection/sampling_deviation                  |stdyDscr/method/dataColl/deviat                                             |Deviations from the Sample Design                                      |
|study_desc/method/data_collection/coll_mode                           |stdyDscr/method/dataColl/collMode                                           |Mode of data collection                                                |
|study_desc/method/data_collection/research_instrument                 |stdyDscr/method/dataColl/resInstru                                          |Type of Research Instrument                                            |
|study_desc/method/data_collection/instru_development                  |stdyDscr/method/dataColl/instrumentDevelopment                              |Instrument development                                                 |
|study_desc/method/data_collection/instru_development_type             |stdyDscr/method/dataColl/instrumentDevelopment/@type                        |Instrument development type                                            |
|study_desc/method/data_collection/sources                             |stdyDscr/method/dataColl/sources                                            |Sources                                                                |
|- name                                                                |                                                                            |Source name                                                            |
|- origin                                                              |                                                                            |Origin of Source                                                       |
|- characteristics                                                     |                                                                            |Characteristics of Source Noted                                        |
|study_desc/method/data_collection/coll_situation                      |stdyDscr/method/dataColl/collSitu                                           |Characteristics of Data Collection Situation - Notes on data collection|
|study_desc/method/data_collection/act_min                             |stdyDscr/method/dataColl/actMin                                             |Supervision                                                            |
|study_desc/method/data_collection/control_operations                  |stdyDscr/method/dataColl/ConOps                                             |Control Operations                                                     |
|study_desc/method/data_collection/weight                              |stdyDscr/method/dataColl/weight                                             |Weighting                                                              |
|study_desc/method/data_collection/cleaning_operations                 |stdyDscr/method/dataColl/cleanOps                                           |Cleaning Operations                                                    |
|study_desc/method/method_notes                                        |stdyDscr/method/notes                                                       |Methodology notes                                                      |
|study_desc/method/analysis_info                                       |stdyDscr/method/anlyInfo                                                    |Data Appraisal                                                         |
|study_desc/method/analysis_info/response_rate                         |stdyDscr/method/anlyInfo/respRate                                           |Response Rate                                                          |
|study_desc/method/analysis_info/sampling_error_estimates              |stdyDscr/method/anlyInfo/EstSmpErr                                          |Estimates of Sampling Error                                            |
|study_desc/method/analysis_info/data_appraisal                        |stdyDscr/method/anlyInfo/dataAppr                                           |Data Appraisal                                                         |
|study_desc/method/study_class                                         |stdyDscr/method/stdyClas                                                    |Class of the Study                                                     |
|study_desc/method/data_processing                                     |stdyDscr/method/dataProcessing                                              |Data Processing                                                        |
|- type                                                                |                                                                            |Data processing type                                                   |
|- description                                                         |                                                                            |Data processing description                                            |
|study_desc/method/coding_instructions                                 |stdyDscr/method/codingInstructions                                          |Coding Instructions                                                    |
|- related_processes                                                   |                                                                            |Related processes                                                      |
|- type                                                                |                                                                            |Coding instructions type                                               |
|- txt                                                                 |                                                                            |Coding instructions text                                               |
|- command                                                             |                                                                            |Command                                                                |
|- formal_language                                                     |                                                                            |Identify the language of the command code                              |
|study_desc/data_access                                                |stdyDscr/dataAccs/setAvail/dataAccs                                         |                                                                       |
|study_desc/data_access/dataset_availability                           |stdyDscr/dataAccs/setAvail                                                  |Data Set Availability                                                  |
|study_desc/data_access/dataset_availability/access_place              |stdyDscr/dataAccs/setAvail/accsPlac                                         |Location of Data Collection                                            |
|study_desc/data_access/dataset_availability/access_place_url          |stdyDscr/dataAccs/setAvail/accsPlac/@URI                                    |URL for Location of Data Collection                                    |
|study_desc/data_access/dataset_availability/original_archive          |stdyDscr/dataAccs/setAvail/origArch                                         |Archive where study is originally stored                               |
|study_desc/data_access/dataset_availability/status                    |stdyDscr/dataAccs/setAvail/avlStatus                                        |Availability Status                                                    |
|study_desc/data_access/dataset_availability/coll_size                 |stdyDscr/dataAccs/setAvail/collSize                                         |Extent of Collection                                                   |
|study_desc/data_access/dataset_availability/complete                  |stdyDscr/dataAccs/setAvail/complete                                         |Completeness of Study Stored                                           |
|study_desc/data_access/dataset_availability/file_quantity             |stdyDscr/dataAccs/setAvail/fileQnty                                         |Number of Files                                                        |
|study_desc/data_access/dataset_availability/notes                     |stdyDscr/dataAccs/setAvail/notes                                            |Notes                                                                  |
|study_desc/data_access/dataset_use                                    |stdyDscr/dataAccs/useStmt                                                   |Data Set Availability                                                  |
|study_desc/data_access/dataset_use/conf_dec                           |stdyDscr/dataAccs/useStmt/confDec                                           |Confidentiality Declaration                                            |
|- txt                                                                 |.                                                                           |Confidentiality declaration text                                       |
|- required                                                            |- required                                                                  |Is signing of a confidentiality declaration required?                  |
|- form_url                                                            |- URI                                                                       |Confidentiality declaration form URL                                   |
|- form_id                                                             |- formNo                                                                    |Form ID                                                                |
|study_desc/data_access/dataset_use/spec_perm                          |stdyDscr/dataAccs/useStmt/specPerm                                          |Special Permissions                                                    |
|- txt                                                                 |                                                                            |Special permissions description                                        |
|- required                                                            |- required                                                                  |Indicate if special permissions are required to access a resource      |
|- form_url                                                            |- URI                                                                       |Form URL                                                               |
|- form_id                                                             |- formNo                                                                    |Form ID                                                                |
|study_desc/data_access/dataset_use/restrictions                       |stdyDscr/dataAccs/useStmt/restrctn                                          |Restrictions                                                           |
|study_desc/data_access/dataset_use/contact                            |stdyDscr/dataAccs/useStmt/contact                                           |Contact                                                                |
|- name                                                                |.                                                                           |Name                                                                   |
|- affiliation                                                         |- affiliation                                                               |Affiliation                                                            |
|- uri                                                                 |- URI                                                                       |URI                                                                    |
|- email                                                               |- email                                                                     |Email                                                                  |
|study_desc/data_access/dataset_use/cit_req                            |stdyDscr/dataAccs/useStmt/citReq                                            |Citation requirement                                                   |
|study_desc/data_access/dataset_use/deposit_req                        |stdyDscr/dataAccs/useStmt/deposReq                                          |Deposit requirement                                                    |
|study_desc/data_access/dataset_use/conditions                         |stdyDscr/dataAccs/useStmt/conditions                                        |Conditions                                                             |
|study_desc/data_access/dataset_use/disclaimer                         |stdyDscr/dataAccs/useStmt/disclaimer                                        |Disclaimer                                                             |
|study_desc/data_access/notes                                          |stdyDscr/dataAccs/setAvail/notes                                            |Notes                                                                  |
|data_files                                                            |                                                                            |                                                                       |
|variables                                                             |                                                                            |                                                                       |
|variable_groups                                                       |                                                                            |Variable groups                                                        |

# Annex 4: Mapping the geographic schema to DCAT/schema.org {-}

[to do]

# Annex 5: Mapping the indicator/time series schema to schema.org {-}

[to do]

# Annex 6: Mapping the table schema to schema.org {-}

[to do]

# Annex 7: Mapping the image schema to Dublin Core, IPTC, and schema.org {-}

[to do]

# Annex 8: Mapping the audio schema to Dublin Core and schema.org {-}

[to do]

# Annex 9: Mapping the video schema to Dublin Core and schema.org {-}

[to do]

# Annex 10: Mapping the research/script schema to Dublin Core and schema.org {-}

[to do]


