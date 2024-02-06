---
output: html_document
---

# The power of rich and structured metadata {#chapter03}

The previous chapter defined the features of an advanced data discoverability and dissemination system. What enables such a system is not only the search algorithms and technology, but also the quality of the metadata available to enable them. Metadata is the "structured information that describes, explains, locates, or otherwise makes it easier to retrieve, use or manage that resource" (Data thesaurus, NIH, https://nnlm/gov/data/thesaurus) 

This chapter describes what metadata is needed, and how it can be organized and improved to enable advanced search and recommender solutions. The core message is that to serve its multiple purposes, metadata must be **rich** and **structured**. In this chapter, we build the case for rich, augmented, structured metadata and for the adoption of metadata standards and schemas. 

## Rich metadata

### Defining rich metadata

*Rich* metadata means metadata that is **detailed** and **comprehensive**. What makes metadata "detailed and comprehensive" is not always easy to define, and is specific to each data type. Microdata and geospatial datasets for example will require much more -- and different-- metadata than a document or an image. Metadata standards and schemas provide data curators with detailed lists of *elements* (or *fields*), specific to each data type, that must or may be provided to document a dataset. The metadata elements included in a standard or schema will typically cover *cataloguing material*, *contextual information*, and *explanatory materials*.

#### Cataloguing material

Cataloguing material includes elements such as a title, a unique (and preferably permanent) identifier for the dataset, a version number and description, as well as information related to the data curation (including who generated the metadata and when, or where and when metadata may have been harvested from an external catalog). This information allows the dataset to be uniquely identified within a collection or catalog, and serves as a bibliographic record of the dataset, allowing it to be properly acknowledged and cited in publications.

#### Contextual information

Contextual information describes the context in which the data were collected and how they were put to use. It enables secondary users to understand the background and processes behind the data production. Contextual information should cover topics such as:

   - What justified or required the data collection (the objectives of the data production exercise);
   - Who or what was being studied (the subject and scope of the data collection);
   - The geographic and temporal coverage of the data;
   - Changes and developments that occurred over time in the data collection methodology and in the dataset, if relevant. For repeated cross-section, panel, or time series datasets, this may include information describing changes in the question text, variable labeling, sampling procedures, or others;
   - What are the key output of the data collection, such as a publication, the design or implementation of a policy or project, etc. 
   - Problems encountered in the process of data production;
   - Other useful information on the life cycle of the dataset.

#### Explanatory material

Explanatory materials are the information that should be created and preserved to ensure the long-term functionality of a dataset and its contents. Explanatory materials include:

   - Information about the **data collection methods**: This should describe the instruments used and methods employed, and how they were developed. For sample datasets, details of the sampling design and sampling frames should be included. It is also useful to include information on any monitoring process undertaken during the data collection as well as details of quality controls.
   - **Technical information**: This information relates to the technical framework and should include the computer system used to generate the data and related files; the software packages with which the files were created.
   - Information about the **structure of the dataset**: For quantitative datasets, this includes a detailed data dictionary describing the structure of the dataset, including information about relationships between individual files or records within the study. For example, in the case of microdata, it should include key variables required for unique identification of subjects across data files (needed to properly merge data files), the number of cases and variables in each file, and the number of files in the dataset. For relational databases, the structure and relations between datasets records and elements should be described.
   - **Variables and values, coding and classification schemes** (for microdata and geospatial data): The documentation should contain an exhaustive list of  variables in the dataset, including a complete explanation and full details about the coding and classifications used for the information allocated to those fields. It is especially important to have blank and missing fields explained and accounted for. It is helpful to identify variables to which standard coding classifications apply, and to record the version of the classification scheme used.
   - Information about **derived variables** (for microdata and geospatial data, and tabulations): Many data producers derive new variables from original data. This may be as simple as grouping raw age (in years) data according to groups of years appropriate for the survey, or it may be much more complex and require the use of sophisticated algorithms. When grouped or derived variables are created, the logic for the grouping or derivation must be clear. Simple grouping, such as for age, can be included within the data dictionary. More complex derivations require other means of recording the information. Sufficient supporting information should be provided to allow an easy link between the core variables used and the resultant variables. In addition, computer algorithms used to create the derivations should be saved together with information on the software.
   - Information on **weighting and grossing** (for sample survey datasets): Weighting and grossing variables must be fully documented, with explanations of the construction of the variables and clear indications of the circumstances in which they should be used. The latter is particularly important when different weights are applied for different purposes.
   - Information on **data sources**: Details about the source from which the data is derived should be included. For example, when the data source consists of responses to survey questionnaires, each question should be carefully recorded in the documentation. Ideally, the text will include a reference to the generated variable(s). It is also useful to explain the conditions under which a question would be asked, including, if possible, the cases to which it applies and, ideally, a summary of response statistics.
   - Information on **confidentiality and anonymization**: It is important to determine whether the data contains any confidential information on individuals, households, organizations, or institutions. If so, such information should be recorded together with any agreement on how to use the data, such as with survey respondents. Issues of confidentiality may restrict the analyses to be undertaken or results to be published, particularly if the data is to be made available for secondary use. If the data were anonymized to prevent identification, it is wise to record the anonymization procedure (taking care of not providing information that would enable a reverse-engineering of the procedure) and its impact on the data, as such modification may restrict subsequent analysis.

### Benefits for data users

#### Finding data

Metadata facilitate the efficient discovery of data within online catalogs. It serves as the informational backbone that search engines rely upon to index and categorize data, greatly influencing the discoverability of relevant content. The richness of metadata enhances the effectiveness of search engines, as it provides detailed descriptors about the nature, source, and characteristics of the data. The more comprehensive and detailed the metadata, the more effectively search engines can assist users in identifying pertinent data. 

#### Understanding and using data

Metadata aid analysts to comprehend and utilize data. Metadata offers insights into the context, structure, and attributes of the data, allowing analysts to interpret and use them accurately. In the absence of a comprehensive description accompanying the data, there is a risk that users may misunderstand or misuse the information, or alternatively opt not to use them at all. Without this contextual information, the user may face challenges in extracting meaningful insights.

#### Assessing data

Good metadata provides analysts with essential information that enables them to assess the reliability, fitness for purpose, and consistency of the data. It offers insights into the source, methodology, and any potential limitations associated with the dataset. For analysts seeking to integrate multiple datasets, robust metadata becomes even more crucial, as it facilitates the evaluation of consistency and compatibility across various sources. The ability to gauge the quality and relevance of the data allows analysts to make informed decisions about its suitability for their specific analytical needs. 


### Benefits for data producers 

#### Credibility

Metadata plays a crucial role in ensuring transparency, auditability, and therefore credibility in the field of statistics and data products. By encompassing both information on the processes involved in generating statistics and data products, as well as details describing the products themselves, metadata serves as an essential tool for users to form well-informed opinions about the quality of the data across various dimensions such as relevance, reliability, and accuracy. Essentially, comprehensive metadata acts as a transparent blueprint, offering insights into the methodology, sources, and any transformations applied during the data generation process. It provides users with the necessary context to assess the robustness of the statistics presented. When organizations make such metadata readily available, it demonstrates a commitment to openness and integrity. Essentially, the philosophy is that if an organization has nothing to hide, the most effective way to communicate that is by publishing thorough and comprehensive metadata alongside the statistics, fostering trust, and reinforcing the credibility of the data products they provide.

#### Quality assurance

Metadata holds immense importance in implementing robust quality assurance, quality control, and quality improvement practices throughout the entire lifecycle of data production and utilization. Evaluating the quality of data extends beyond assessing the dataset alone; it encompasses a thorough examination of the processes that culminated in their availability. Comprehensive metadata detailing both the processes and the resulting products becomes indispensable in this context. By offering a detailed account of the methods, sources, and any transformations applied during data generation, metadata becomes a vital tool for quality assurance, enabling thorough scrutiny of the dataset's reliability and accuracy. Equally significant is the role metadata plays in quality control, allowing for the identification and rectification of potential issues in the data production process. Moreover, metadata serves as a foundation for continuous quality improvement, providing insights into areas where enhancements can be made to elevate the overall data quality, thereby ensuring the credibility and utility of the data.

#### Harmonization of data collection

For organizations engaged in data collection and generation, the establishment of a comprehensive meta-database facilitates the harmonization of data collection and processing methods and instruments. Metadata plays a key role in identifying differences, inconsistencies, and the absence of standardized practices across diverse datasets. By centralizing metadata, organizations can create a unified framework that facilitates a systematic understanding of the various data sources and their characteristics. This harmonization is particularly crucial for maintaining consistency and accuracy in statistical reporting. A compelling case for the utilization of metadata in this manner can be found in ["The Struggle for Integration and Harmonization of Social Statistics in a Statistical Agency - A Case Study of Statistics Canada"](https://www.ihsn.org/sites/default/files/resources/IHSN-WP004.pdf) by Gordon Priest (2010), which describes the challenges and benefits of integrating social statistics by fostering a cohesive and standardized approach to data collection and processing within a statistical agency.

#### Visibility

Increase the online visibility of the data, and thus the demand for, and use of the data.

Data cataloguing applications provide search and filtering tools to help users of the catalog identify data of interest. But not all users will start their search for data directly in specialized data catalogs; many will start their search in Google, Google Dataset Search, Bing, Yahoo! or another search engine. 

In some cases, the user may not be brought to the data catalog at all, if the catalog ranked low in the relevance order of the Google query results. [User behavior data (2020)](https://www.smartinsights.com/search-engine-marketing/search-engine-statistics/) showed that "only 9% of Google searchers make it to the bottom of the first page of the search results", and that "only .44% of searchers go to the second page of Google’s search results". It is thus critical to optimize the visibility of the content of specialized data catalogs in the lead search engines, Google in particular. This optimization process is referred to as **search engine optimization** or SEO. [Wikipedia](https://en.wikipedia.org/wiki/Search_engine_optimization) describes SEO as “the process of improving the quality and quantity of website traffic to a website or a web page from search engines. SEO targets unpaid traffic (known as "natural" or "organic" results) rather than direct traffic or paid traffic. (…) As an Internet marketing strategy, SEO considers how search engines work, the computer-programmed algorithms that dictate search engine behavior, what people search for, the actual search terms or keywords typed into search engines, and which search engines are preferred by their targeted audience. SEO is performed because a website will receive more visitors from a search engine when websites rank higher on the search engine results page.” 

:::quote
Because search engines crawl the web pages that are generated from databases (rather than crawling the databases themselves), your carefully applied metadata inside the database will not even be seen by search engines unless you write scripts to display the metadata tags and their values in HTML meta tags. It is crucial to understand that any metadata offered to search engines must be recognizable as part of a schema and must be machine-readable, which is to say that the search engine must be able to parse the metadata accurately. (For example, if you enter a bibliographic citation into a single metadata field, the search engine probably won’t know how to distinguish the article title from the journal title, or the volume from the issue number. In order for the search engine to read those citations effectively each part of the citation must have its own field. (...) Making sure metadata is machine-readable requires patterns and consistency, which will also prepare it for transformation to other schema. (This is far more important than picking any single metadata schema. (...) *From the blog post "Metadata, Schema.org, and Getting Your Digital Collection Noticed" by Patrick Hogan (https://www.ala.org/tools/article/ala-techsource/metadata-schemaorg-and-getting-your-digital-collection-noticed-3)*
:::

The ranking of web pages by Google and other lead search engines is determined by complex, proprietary, and non-disclosed algorithms. The only option for a web developer to ensure that a web page appears on top of the Google list of results is to pay for it, publishing it as a "sponsored" link. Otherwise, the ranking of a web page will be determined by a combination of known and unknown criteria. "Google's automated ranking systems are designed to present helpful, reliable information that's primarily created to benefit people, not to gain search engine rankings, in the top Search results." ([Google Search Central](https://developers.google.com/search/docs/fundamentals/creating-helpful-content)) But Google, Bing and other search engines provide web developers with some guidance and recommendations on search engine optimization (SEO). See for example the [Google Search Central](https://developers.google.com/search) website where Google publish "Specific things you can do to improve the SEO of your website". 

   - [Google Search Engine Optimization Starter Guide](https://developers.google.com/search/docs/beginner/seo-starter-guide)
   - [Google Dataset Search, Advanced SEO](https://developers.google.com/search/docs/data-types/dataset)
   - [Bing webmaster Tools](https://www.bing.com/webmasters/about)

Improving the ranking of catalog pages is a shared responsibility of data curators and catalog developers and administrators. **Data curators** must pay particular attention to providing rich, useful content in the catalog web pages (the HTML pages that describe each catalog entry). To identify relevant results, search engines index the content of web pages. Datasets that are well documented, i.e. those published with rich and structured metadata, will thus have a better chance to be discovered. Much attention should be paid to some core elements including the dataset title, producer, description (abstract), keywords, topics, access license, and geographic coverage. In Google Search Central's terms, curators must "create helpful, reliable, people-first content" (not search engine-first content) and "use words that people would use to look for your content, and place those words in prominent locations on the page, such as the title and main heading of a page, and other descriptive locations such as alt text and link text.* 

**Developers and administrators of cataloguing applications** must pay attention to other aspects of a catalog that will make it rank higher in Google and other search engine results: 

- Ensuring that a data catalog delivers a good experience to users (see [Understanding page experience in Google Search results](https://developers.google.com/search/docs/appearance/page-experience)), which among other things involves:
   - Catalog pages that load fast
   - Catalog pages that are mobile-friendly. A data catalog should thus be built with a responsive design.
   - Provide secure connection by serving the catalog over HTTPS (see more information, see for example https://web.dev/enable-https/)
- Embedding *structured data* in the catalog's HTML pages. The HTML pages in a data catalog are mostly the pages that will make the metadata specific to an entry visible to the user. These pages are automatically generated by the cataloguing application, by extracting and formatting the metadata stored in the catalog's database. Structured data is information that will be included in these HTML pages (but not shown to the user) to help Google understand the content of the page. The use of *structured data* only applies to certain types of content, including datasets. The use of structured data influences not only the ranking of a page, but also the way information on the page will be displayed by Google. The next section is dedicated to this.

Last, Google will "reward" popular websites, i.e. websites that are frequently visited and to which many other influent and popular websites provide links. Google's recommendation is thus to "tell people about your site. Be active in communities where you can tell like-minded people about your services and products that you mention on your site."

A helpful and detailed [self-assessment list](https://developers.google.com/search/docs/fundamentals/creating-helpful-content) of items that data curators, catalog developers, and catalog administrators should pay attention to is provided by Google. Various tools are also available to catalog developers and administrators to assess the technical performance of their websites.

#### Cost-effectiveness of data dissemination

Publishing detailed metadata proves to be a cost-effective strategy for organizations involved in data dissemination. By providing comprehensive information about the datasets, including their sources, methodologies, and limitations, organizations empower users to independently navigate and understand the data. This transparency reduces the burden on the organization to respond to frequent and varied user requests for additional information. When users can access detailed metadata, they gain the insights needed to interpret and utilize the data effectively, minimizing the necessity for additional clarifications or support. This, in turn, streamlines the operation of a data dissemination service, saving resources that would otherwise be allocated to addressing individual inquiries. Essentially, the proactive disclosure of comprehensive metadata serves as a preemptive measure, contributing to a more efficient and cost-effective dissemination process by equipping users with the information required for autonomous and accurate data interpretation.

#### Preservation of institutional memory

The meticulous production and preservation of detailed metadata by organizations involved in data collection, generation, processing, and analysis, such as national statistics offices, play a pivotal role in supporting the preservation of institutional memory. Detailed metadata serve as a comprehensive record documenting the intricacies of data collection methodologies, processing techniques, and analytical approaches employed over time. This wealth of information helps to safeguard the institutional memory by providing future generations of analysts and data stewards with insights into past practices, standards, and decision-making processes. It acts as a knowledge repository, allowing the organization to learn from historical experiences, maintain consistency in methodologies, and ensure a coherent and informed evolution of data-related practices. Detailed metadata function as a vital component of institutional memory preservation, enabling continuity, learning, and informed decision-making within organizations engaged in the multifaceted aspects of data management.


## Structured metadata

### Defining structured metadata

Metadata should not only be comprehensive and detailed, they should also be organized in a **structured** manner, preferably using a standardized structure. **Structured metadata** means that the metadata are stored in specific *fields* (or *elements*) organized in a <u>metadata schema</u>. **Standardized** means that the list and description of elements are commonly agreed by a community of practice, in which case the metadata schema is referred to as a metadata standard. Some metadata schemas may be standard within an organization, others may be adopted by a larger community of practice, in some cases internationally. International metadata standards have particular value as they facilitate the sharing of international good practice and support cost-effective and efficient data and metadata exchange. 

Some metadata standards have originated from academic data centers, like the [Data Documentation Initiative (DDI)](https://ddialliance.org/), maintained by the [Inter-University Consortium for Political and Social Research](https://www.icpsr.umich.edu/web/pages/) (ICPSR) at the University of Michigan. Other found their origins in specialized communities of practice (like the [ISO 19139](https://www.iso.org/standard/67253.html?browse=tc) for geospatial resources). The private sector also contributes to the development of standards, like the [International Press Telecommunications Council (IPTC)](https://iptc.org/) standard developed by and for news media.

Metadata compliant with standards will typically be stored as JSON or XML files (described in Chapter 2), which are plain text files. The example below show how a simple free-text content would be structured and stored in JSON and XML formats, using metadata elements from the [DDI Codebook](https://ddialliance.org/Specification/DDI-Codebook/2.5/) metadata standard: 

**Free text version**: 

*The Child Mortality Survey (CMS) was conducted by the National Statistics Office of Popstan from July 2010 to June 2011, with financial support from the Child Health Trust Fund (TF123_456).*

**Structured, machine-readable (JSON) version**:


```json
{
  "title"           : "Child Mortality Survey 2010-2011",
  "alternate_title" : "CMS 2010-2011", 
  "authoring_entity": "National Statistics Office (NSO)", 
  "funding_agencies": [{"name":"Child Health Trust Fund (CHTF)", "grant":"TF123_456"}],
  "coll_dates"      : [{"start":"2010-07", "end":"2011-06"}],
  "nation"          : [{"name":"Popstan", "abbreviation":"POP"}] 
}  
```

In XML format (with DDI tag names): 

```xml
<titl>Child Mortality Survey 2010-2011</titl>
<altTitl>CMS 2010-2011</altTitl>
<rspStmt><AuthEnty>National Statistics Office</AuthEnty></rspStmt>
<fundAg abbr=CHTF>Child Health Trust Fund</fundAg>
<collDate date="2010-07" event="start"/>
<collDate date="2011-06" event="end"/>
<nation abbr="POP">Popstan</nation>
```

All three versions contain (almost) the same information. In the structured version, we have added acronyms and the ISO country code. This does not create new information but will help make the existing information more discoverable and inter-operable. The structured version is clearly more suitable for publishing in a meta-database (or catalog). Organizing and storing metadata in such a structured manner will enable all kinds of applications. For example, when metadata for a collection of surveys are stored in a database, it becomes straightforward to apply filters (for example, a filter by country using the nation/name element) and targeted searches to answer questions like "What data are available that cover the month of December 2010?" or "What surveys did the CHTF sponsor?". 
                                                   
### Formats for structured metadata: JSON and XML 

Metadata standards and schemas consist of structured lists of metadata fields. They serve multiple purposes. First, they help data curators generate complete and usable documentation of their datasets. Metadata standards that are intuitive and *human-readable* better serve this purpose. Second, they help generate *machine-readable* metadata that are the input to software applications like on-line data catalogs. Metadata available in open file formats like JSON (JavaScript Object Notation) and XML (eXtended Markup Language) are most suitable for this purposes.

Some international metadata standards like the **Data Documentation Initative** (DDI Codebook, for microdata), the ISO 19139 (for geospatial data), or the Dublin Core (a more generic metadata specification) are described and published as XML specifications. Any XML standard or schema can be "translated" into JSON, which is our preferred format (a choice we justify in the next section). 

JSON and XML formats have similarities: 

   - Both are non-proprietary text files
   - Both are hierarchical (they may contain values within values)
   - Both can be parsed and used by many programming languages including R and Python

JSON files are however easier to parse than XML, easier to generate programmatically, and easier to read by humans. This makes them our preferred choice for describing and using metadata standards and schemas.

Metadata in JSON are stored as *key/value* pairs, where the keys correspond to the names of the metadata elements in the standard. Values can be string, numeric, boolean, arrays, null, or JSON objects (for a more detailed description of the JSON format, see [www.w3schools.com](https://www.w3schools.com/js/js_json_intro.asp)). Metadata in XML are stored within named tags. The example below shows how the JSON and XML formats are used to document the list of authors of a [document](http://hdl.handle.net/10986/34511), using elements from the Dublin Core metadata standard.

<center>
![](./images/document_example_01b_authors_keywords.JPG){width=100%}
</center>
<br>

In the *documents* schema, authors are documented in the metadata element `authors` which contains the following sub-elements: `first_name`, `initial`, `last_name`, and `affiliation`.

<center>
![](./images/JSON_array_list_authors.JPG){width=100%}
</center>
<br>

In JSON, this information will be stored in key/value pairs as follows. 


```json
"authors" : [
  {"first_name" : "Dieter", 
   "last_name"  : "Wang", 
   "affiliation": "World Bank Group; Fragility, Conflict and Violence"},
  {"first_name" : "Bo",     
   "initial"    : "P.J.", 
   "last_name"  : "Andrée", 
   "affiliation": "World Bank Group; Fragility, Conflict and Violence"},
  {"first_name" : "Andres", 
   "initial"    : "F.", 
   "last_name"  : "Chamorro", 
   "affiliation": "World Bank Group; Development Data Analytics and Tools"},
  {"first_name" : "Phoebe", 
   "initial"    : "G.", 
   "last_name"  : "Spencer",  
   "affiliation":"World Bank Group; Fragility, Conflict and Violence"}
]
```

In XML, the same information will be stored within named tags as follows. 


```xml
<authors>
  <author>
    <first_name>Dieter</first_name> 
    <last_name>Wang</last_name> 
    <affiliation>World Bank Group; Fragility, Conflict and Violence</affiliation>
  </author>
  <author>
    <first_name>Bo</first_name> 
    <initial>P.J.</initial> 
    <last_name>Andrée</last_name> 
    <affiliation>World Bank Group; Fragility, Conflict and Violence</affiliation>
  </author>
  <author>
    <first_name>Andres</first_name> 
    <initial>E.</initial>
    <last_name>Chamorro</last_name> 
    <affiliation>World Bank Group; Development Data Analytics and Tools</affiliation>
  </author>
  <author>
    <first_name>Phoebe</first_name> 
    <initial>G.</initial>
    <last_name>Spencer</last_name> 
    <affiliation>World Bank Group; Fragility, Conflict and Violence</affiliation>
  </author>
</authors>
```

### Benefits of structured metadata

Metadata standards and schemas must be comprehensive and intuitive. They aim to provide comprehensive and granular lists of elements. Some standards contain a very long list of elements. Most often, only a subset of the available elements will be used to document a specific dataset. For example, the elements of the DDI metadata standard related to sample design will be used to document sample survey datasets but will be ignored when documenting a population census or an administrative dataset. In all standards and schemas, most elements are *optional*, not *required*. Data curators should however try and provide content for all elements for which information is or can be made available.

Complying with metadata standards and schemas contributes to the completeness, usability, discoverability, and inter-operability of the metadata, and to the visibility of the data and metadata.

#### Completeness 

When they document datasets, data curators who do not make use of metadata standards and schemas tend to focus on the readily-available documentation and may omit some information that secondary data users --and search engines-- may need. Metadata standards and schemas provide checklists of what information could or should be provided. These checklists are developed by experts, and are regularly updated or upgraded based on feedback received from users or to accommodate new technologies. 

Generating complete metadata will often be a collaborative exercise, as the production of data involves multiple stakeholders. The implementation of a survey, for example, may involve sampling specialists, field managers, data processing experts, subject matter specialists, and programmers. Documenting a dataset should not be seen as a last and independent step in the implementation of a data collection or production project. Ideally, metadata will be captured continuously and in quasi-real time during the entire life cycle of the data collection/production, and contributed by those who have most knowledge of each phase of the data production process. 

Generating complete and detailed metadata may be seen as a burden by some organizations or researchers. But it will typically represent only a small fraction of the time and budget invested in the production of the data, and is an investment that will add much value to the data by increasing their usability and discoverability.
 
#### Usability 

Fully understanding a dataset before conducting analysis should be a pre-requisite for all researchers and data users. But this will only be possible when the documentation is easy to obtain and exploit. Convenience to users is key. When using a geographic dataset for example, the user should be able to immediately find the coordinate reference system that was used. When using survey microdata, which may contain hundreds or thousands of variables, the user need to be able to immediately access information on a variable label, underlying question, universe, categories, etc. Structured metadata enables such "convenience", as they can easily be transformed into bookmarked PDF documents, searchable websites, machine-readable codebooks, etc. The way metadata are displayed can be tailored to the specific needs of different categories of users.

#### Discoverability

:::quote
Data discoverability is one of the main tasks, next to availability and interoperability, that public policy makers and implementers should take into due consideration in order to foster access, use and re-use of public sector information, particularly in case of open data. Users shall be enabled to easily search and find data they need for the most different purposes. That is clearly highlighted in the introduction statements of the INSPIRE Directive, where we can read that “The loss of time and resources in searching for existing (spatial) data or establishing whether they may be used for a particular purpose is a key obstacle to the full exploitation of the data available”.
From [*Metadata and data portals/catalogues are essential assets to enable that data discoverability.*](https://www.europeandataportal.eu/en/impact-studies/country-insights/italy/italy-discoverability-practice)
:::

What matters is not only <u>what</u> metadata are provided as input to the search engines that matters, it is also <u>how</u> the metadata are provided. To understand the value of structured metadata, we need to take into consideration how search engines ingest, index, and exploit the metadata. In brief, the metadata will need to be acquired, augmented, analyzed and transformed, and indexed before they can be made searchable. We provide here an overview of the process, which is described in detail by D. Turnbull and J. Berryman in ["Relevant Search: With applications for Solr and Elasticsearch"](https://www.manning.com/books/relevant-search) (2016). 

- **Acquisition**: Search engines like Google and Bing acquire metadata by crawling billions of web pages using *web crawlers* (or *bots*), with an objective to cover the entire web. Guidance is available to webmasters on how to optimize websites for visibility (see for example [Google's Search Engine Optimization (SEO) Starter Guide](https://developers.google.com/search/docs/beginner/seo-starter-guide). The search tools embedded in specialized data catalogs have a much simpler task, as the catalog administrators and curators generate or control, and provide, the well-contained content to be indexed. In a cataloguing application like NADA, this content is provided in the form of *structured metadata files* saved in JSON or XML format. For textual data (documents), the content of the document (not only the metadata on the) can also be indexed. The process of acquisition/extraction of metadata by the search engine tool must preserve the structure of the metadata, in its original or in a modified form. This will be critical for optimizing the performance of the search tool and the ranking of query results (e.g., a keyword found in a document title may have more weight than the same keyword found in the document abstract), for implementing facets, or for providing advanced search options (e.g., search only in the "authors" metadata field).  

- **Augmentation** or **enrichment**: the content of the metadata can be *augmented* or *enriched* in multiple ways, often automatically (by extracting information from an external source, or using machine learning algorithms). Part of this augmentation process should happen before the metadata are submitted to the search engine. Other procedures of enrichment of the metadata may be implemented after acquisition of the metadata by the search engine tool. Metadata augmentation can have a significant impact on the discoverability of data. See the section "Augmented (enriched) metadata" below.

- **Analysis** or **transformation**: The metadata generated by the data curator and by the augmentation process will mostly (not exclusively) consist of text. For the purpose of discoverability, some of the text has no value; words like "the", "a", it", "with", etc., referred to as *stop words*, will be removed from the metadata (multiple tools are available for this purpose). The remaining words will be converted to lowercase, may be submitted to spell checkers (to exclude or fix errors), and words will be *stemmed* or *lemmatized*. The stemming or lemmatization consist of converting words to their *stem* or *root*); this will among other transformations change plurals to singular and the conjugated forms of the verbs to their base form. Last, the transformed metadata will be *tokenized*, i.e. split into a list of terms (*tokens*). To enable semantic searchability, the metadata can also be converted into numeric vectors using natural language processing *embedding* models. These vectors will be saved in a database (such as [ElasticSearch](https://github.com/elastic/elasticsearch) or [Milvus](https://milvus.io/)) that will provide functionalities to measure similarity/distance between vectors. Section 1.8 below provide more information on text embedding and semantic searchability.

- **Indexing**: The last phase of metadata processing is the indexing of the tokens. The index of a search engine is an *inverted index*, which will contain a list of all terms found in the metadata, with the following information (among other) attached to each term:
   - The *document frequency*, i.e. the number of metadata documents where the word is found (a *metadata document* is the metadata related to one dataset).
   - The identification of the metadata documents in which the term was found.
   - The *term frequency* in each metadata document. 
   - The *term positions* in the metadata document, i.e. where the term is found in the document. This is important to identify colocations. When a user submits a query for "demographic transition" for example, documents where the two terms are found next to each other will be more relevant than documents where both terms appear but in different parts of the document.

Once the metadata has been acquired, transformed, and indexed, it is available for use via a user interface (UI). A data catalog UI will typically include a search box and facets (filters). The search engine underlying the search box can be simple (out-of-the-box full text search, looking for exact matches of keywords), or advanced (with semantic search capability and optimized ranking of query results). Basic full-text search do not provide satisfactory user experience, as we illustrated in the introduction to this Guide. Rich, structured metadata, combined with advanced search optimization tools and machine learning solutions, allow catalog administrators to tune the search engine, and implement advanced solutions including semantic searchability.  

<center>
![](./images/schema_documentation_indexing.JPG){width=100%}
</center>

#### Interoperability 

Data catalogs that adopt common metadata standards and schemas can exchange information including through automated harvesting and synchronization of catalogs. This allows them to increase their visibility, and to publish their metadata in hubs. Recommendations and guidelines for improved inter-operability of data catalogs are provided by the [Open Archives Initiative](https://www.openarchives.org/). 

Interoperability between data catalogs can be further improved by the adoption of common controlled vocabularies. For example, the adoption of the ISO country codes in country lists will guarantee that all catalogs will be able to filter dataset by country in a consistent manner. This will solve the issue of possible differences in the spelling of country names (e.g., one catalog referring to the *Democratic Republic of Congo* as *Congo, DR*, and another one as *Congo, Dem. Rep.*). It also solves issues of changing country names, e.g. *Swaziland* renamed as *Eswatini* in 2018). Controlled vocabularies are often used for "categorical" metadata elements like topics, keywords, data type, etc. Some metadata standards like the ISO 19139 for geospatial data include their own recommended controlled vocabularies. Ideally, controlled vocabularies are developed in accordance with [FAIR principles](https://www.go-fair.org/fair-principles/) (Findability, Accessibility, Interoperability, and Reuse of digital assets). "The principles emphasise machine-actionability (i.e., the capacity of computational systems to find, access, interoperate, and reuse data with none or minimal human intervention) because humans increasingly rely on computational support to deal with data as a result of the increase in volume, complexity, and creation speed of data." (https://www.go-fair.org/fair-principles/) 

The adoption of standards and schemas by software developers also contributes to the easy transfer of metadata across applications. For example, data capture tools like [Survey Solutions](https://mysurvey.solutions/en/) by the World Bank and [CsPro](https://www.census.gov/data/software/cspro.html) by the US Census Bureau offer options to export metadata compliant with the DDI Codebook standard; ESRI's ArcGIS software export geospatial metadata in the ISO 19139 standard. 


## Recommended standards

The standards we recommend and describe in this guide are the following: 

| Data type                  | Standard                                        | 
| -------------------------- | ----------------------------------------------- | 
| Documents                  | Dublin Core Metadata Initiative (DCMI), MARC    | 
| Microdata                  | Data Documentation Initiative 2.5 (Codebook)    | 
| Geographic datasets and services | ISO 19110, ISO19115, ISO19119, ISO 19139  | 
| Time series, Indicators    | Custom-designed schema                          | 
| Statistical tables         | Custom-designed schema                          | 
| Photos / Images            | IPTC (for advanced use) or Dublin Core augmented| 
| Audio files                | Dublin Core augmented with AudioObject from schema.org | 
| Videos                     | Dublin Core augmented with VideoObject from schema.org | 
| Programs and scripts       | Custom-designed schema                          | 
| External resources         | Dublin Core                                     |
| All data types             | schema.org and DCAT  (used for search engine optimization purpose, not as the primary schema to document resources)|

<br>


### Documents

**Documents** are bibliographic resource of any type, such as books, working papers and papers published in scientific journals, reports, manuals, and other resources consisting mainly of text. Document libraries have along tradition of using structured metadata to manage their collections, which dates back from before the days this was computerized. Multiple standards are available. The Dublin Core Metadata Initiative specification (DCMI) provides simple and flexible option. The MARC standard (**MA**chine-**R**eadable **C**ataloging) standard used by the United States Library of Congress is another, more advanced one. The schema we describe in this Guide make is the DCMI complemented by a few elements inspired by the MARC standard.

### Microdata

**Microdata** are <u>unit-level</u> data on a population of individuals, households, dwellings, facilities, establishments or other. Microdata are typically obtained from surveys, censuses, or administrative recording systems. To document microdata, the Data Documentation Initiative (DDI) Alliance has developed the DDI metadata standard. "The Data Documentation Initiative (DDI) is an international standard for describing the data produced by surveys and other observational methods in the social, behavioral, economic, and health sciences. DDI is a free standard that can document and manage different stages in the research data lifecycle, such as conceptualization, collection, processing, distribution, discovery, and archiving. Documenting data with DDI facilitates understanding, interpretation, and use -- by people, software systems, and computer network." (Source: https://ddialliance.org/, accessed on 7 June 2021)

The DDI standard comes in two versions: DDI Codebook and DDI Lifecycle. 

   - [DDI-Codebook](https://ddialliance.org/Specification/DDI-Codebook/2.5/) is a light-weight version of the standard. Its elements include descriptive content for variables, files, source material, and study level information. The standard is designed to support the discovery, preservation, and the informed use of data.
   - [DDI Lifecycle](https://ddialliance.org/Specification/DDI-Lifecycle/3.3/) is designed to document and manage data across the entire life cycle, from conceptualization to data publication, analysis and beyond. It encompasses all of the DDI-Codebook specification and extends it. 
   
In this Guide, which focuses on the use of matadata standards for documentation, cataloguing and dissemination purposes, we recommend the use of the DDI Codebook which is much easier to implement than the DDI LifeCycle. DDI Codebook provides all necessary elements needed for our purpose of improving data discoverability and usability. 

### Geographic datasets, data structures, and data services

Geographic data identify and depict geographic locations, boundaries and characteristics of features on the surface of the earth. **Geographic datasets** include raster and vector data files. More or more data is disseminated not in the form of datasets, but in the form of **geographic data services** mainly via web applications. The ISO Technical Committee on Geographic Information/Geomatics (ISO/TC211), created a set of metadata standards to describe geographic datasets (ISO 19115), the geographic data structures of vector data (ISO 19110), and geographic data services (ISO 19119). These ISO standards are also available as an XML specification, the ISO 19139. In this Guide, we describe a JSON and simplified --but ISO-compatible-- version of this complex schema. 

### Time series, indicators

**Indicators** are summary (or "aggregated") measures related to a key issue or phenomenon and derived from a series of observed facts. For example, the *school enrollment rate* indicator can be obtained from survey or census microdata, and the *GDP per capita* indicator is the output of a complex national accounting process that exploits many sources. When an indicator is repeated over time at a regular frequency (annual, quarterly, monthly or other), and when the time dimension is attached to its values, we obtain a **time series**. National statistical agencies and many other organizations publish indicators and time series. Some well-known public databases of time series indicators include the World Bank's [World Development Indicators (WDI)](https://datatopics.worldbank.org/world-development-indicators/), the Asian Development Bank's [Key Indicators (KI)](https://www.adb.org/publications/series/key-indicators-for-asia-and-the-pacific), and the United Nations Statistics Division [Sustainable Development Goals (SDG) database](https://unstats.un.org/sdgs/indicators/database/). Some databases provide indicators that are not time series, like the Demographic and Health Survey (DHS) [StatCompiler](https://www.statcompiler.com/en/). Time series and indicators must be published with metadata that provide information on their spatial and temporal coverage, definition, methodology, sources, and more. No international standard is available to document indicators and time series. The JSON metadata schema we describe in this guide was developed by compiling a list of metadata elements found in international indicators databases, complemented with elements from other metadata schemas. 

### Statistical tables

**Statistical tables** (or *cross tabulations* or *contingency tables*) are summary presentations of data, presented as arrays of rows and columns that display numeric aggregates in a clearly labeled fashion. They are typically found in publications such as statistical yearbooks, census and survey reports, research papers, or published on-line. We developed the metadata schema presented in this Guide based on a review of a large collection of tables and of the 2015 [W3C Model for Tabular Data and Metadata on the Web](https://www.w3.org/TR/tabular-data-model/#bib-tabular-metadata). This schema is intended to facilitate the cataloguing and discovery of tabular data, not to provide an electronic solution to automatically reproduce tables.

### Images

The **images** we are interested in are photos and images available in electronic format. Some images are generated using digital cameras and are "born digital". Others may have been created by scanning photos, or using other techniques. Note that satellite and remote sensing imagery are not considered in this Guide as images, but as geospatial (raster) data which should be documented using the ISO 19139 schema. To document images, we suggest two options: the [Dublin Core Metadata Initiative](https://dublincore.org/) standard augmented by some [ImageObject (from schema.org)](https://schema.org/ImageObject) elements as a simple option, and the IPTC standard for more advanced uses and users.  

### Audio 

To document and catalog audio recordings, we propose a simple metadata schema that combines elements of the [Dublin Core Metadata Initiative](https://dublincore.org/) and of the [AudioObject (from schema.org)](https://schema.org/AudioObject) schemas.

### Videos

To document and catalog videos, we propose a simple metadata schema that combines elements of the [Dublin Core Metadata Initiative](https://dublincore.org/) and of the [VideoObject (from schema.org)](https://schema.org/VideoObject) schemas.

### Programs and scripts

We are interested in documenting and disseminating **data processing and analysis programs and scripts**. By “programs and scripts” we mean the code written to conduct data processing and data analysis, that results in the production of research and knowledge products including dublications, derived datasets, visualizations, or other. These scripts are produced using statistical analysis software or programming languages like [R](https://www.r-project.org/), Python, [SAS](https://www.sas.com/en_us/software/stat.html), [SPSS](https://www.ibm.com/products/spss-statistics), [Stata](https://www.stata.com/) or equivalent. There are multiple reasons to invest in the documentation and dissemination of reproducible and replicable data processing and analysis (see chapter 12). Increasingly, the dissemination of reproducible scripts is a condition imposed by peer-reviewed journals to authors of papers they publish. Data catalogs should be the go-to place for those who look for reproducible research and examples of good practice in data analysis. As no international metadata schema is available to document and catalog scripts, we developed a schema for this purpose.

### External resources

**External resources** are files and links that we may want to attach to a dataset's published metadata in a data catalog. When we publish metadata in a catalog, what is published is only the textual documentation contained in the JSO or XML metadata file. Other resources attached to a dataset (such as the questionnaire for a survey, technical or training manuals, tabulations, reports, possibly micro-data files, etc.) are not included in these metadata, but also constitute important materials for data users. All these resources are what we consider as *external resources* ("external" to the schema-compliant metadata), which need to be catalogued and (for most of them) published with the metadata. A simple metadata schema, based on the Dublin Core, is used to provide some essential information on these resources.     


## A note on other standards

### SDMX

The metadata standards and schemas described in the Guide do not include the [Statistical Data and Metadata eXchange (SDMX)](https://sdmx.org/?sdmx_news=launching-the-new-sdmx-3-0-standard) standard sponsored by a group of international organisations. Although SDMX includes a metadata component, it is intended to support machine-to-machine data exchange, not data documentation and discoverability. SDMX and the metadata standards and schemas we describe in the Guide can --and should-- be made inter-operable. 

### schema.org and DCAT

*Structured data* is information that is embedded in HTML pages that helps Google classify, understand, and display the content of the page when the page is related to a specific type of content. The information stored in the structured data does not impact how the page itself is displayed in a web browser; it only impacts the display of information on the page when returned by Google search results. The types of content to which structured metadata applies is diverse and includes items like job positings, cooking receipes, books, events, movies, math solvers, and others (see the list provided in [Google's Search Gallery](https://developers.google.com/search/docs/appearance/structured-data/search-gallery)). It also applies to resources of type *dataset* and *image*. In this context, a *dataset* can be any type of structured dataset including microdata, indicators, tables, and geographic datasets.

The *structured data* to be embedded in an HTML page consists of a set of metadata elements compliant with either the [*dataset* schema from schema.org](https://schema.org/Dataset) or W3C's Data Catalog Vocabulary ([DCAT](https://www.w3.org/TR/vocab-dcat/#dcat-scope)) for datasets, and with the *image* schema from schema.org for images. For datasets, the schema.org schema is the most frequently used option.[^1] 

   - **schema.org**: [schema.org](www.schema.org) is a collection of schemas designed to document many types of resources. The most generic type is a "thing" which can be a person, an organization, an event, a creative work, etc. A *creative work* can be a book, a movie, a photograph, a data catalog, a dataset, etc. Among the many types of *creative work* for which schemas are available, we are particularly interested in the ones that correspond to the types of data and resources we recommend in this guide. This includes:
      - [**DataCatalog**](https://schema.org/DataCatalog): A data catalog is a collection of datasets.  
      - [**Dataset**](https://schema.org/Dataset): A body of structured information describing some topic(s) of interest.  
      - [**MediaObject**](https://schema.org/MediaObject): A media object, such as an image, video, or audio object embedded in a web page or a downloadable dataset. This includes:
         - [**ImageObject**](https://schema.org/ImageObject): An image file.   
         - [**AudioObject**](https://schema.org/AudioObject): An audio file.   
         - [**VideoObject**](https://schema.org/VideoObject): A video file.   
      - [**Book**](https://schema.org/Book): A book.  
      - [**DigitalDocument**](https://schema.org/DigitalDocument): An electronic file or document.  <br>

The schemas proposed by schema.org have been developed primarily "to improve the web by creating a structured data markup schema supported by major search engines. On-page markup helps search engines understand the information on web pages and provide richer search results." (from [schema.org, Q&A](https://schema.org/docs/faq.html#0)) These schemas have not been developed by specialized communities of practice (statisticians, survey specialists, data librarians) to document datasets for preservation of institutional memory, to increase transparency in the data production process, or to provide data users with the "cook book" they may need to safely and responsibly use data. These schemas are not the ones that statistical organizations need to comply with international recommendations like the Generic Standard Business Process Model (GSBPM). But they play a critical role in improving data discoverability, as they provide webmasters and search engines with a means to better capture and index the content of web-based data platforms. Schemas from schema.org should thus be embedded in data catalogs. Data cataloguing applications should automatically map (some of) the elements of the specialized metadata standards and schemas they use to the appropriate fields of schema.org. Recommended mapping between the specialized standards and schemas and schema.org are not yet available. The production of such mappings, and the development of utilities to facilitate the production of content compliant with schema.org, would contribute to the objective of visibility and discoverability of data.  <br>

   - **DCAT**: [DCAT](https://www.w3.org/TR/vocab-dcat-2/) describes datasets and data services using a standard model and vocabulary. It is organized in 13 "classes" (Catalog, Cataloged Resource, Catalog Record, Dataset, Distribution, Data Service, Concept Scheme, Concept, Organization/Person, Relationship, Role, Period of Time, and Location). Within classes, *properties* are used as metadata elements. For example, the class *Cataloged Resource* includes properties like *title*, *description*, *resource creator*; the class *Dataset* includes properties like *spatial resolution*, *temporal coverage*; many of these properties can easily be mapped to equivalent elements of the specialized metadata schemas we recommend in this Guide.

The embedding of structured metadata (schema.org or DCAT) into HTML pages must be automated in a data cataloguing tool. Data catalogs applications dynamically generate the HTML pages that display the description of each catalog entry. They do so by extracting the necessary metadata from the catalog database, and applying "transformations and styles" to this content to produce a user-friendly output that catalog visitors will view in their web browser. To embed structured data in these pages, the catalog application will (i) extract the relevant subset of metadata elements from the original metadata (e.g., from the DDI-compliant metadata for a micro-dataset), (ii) map these extracted elements to the schema.org or DCAT schema, and (iii) save it in the HTML page as a JSON-LD "hidden" component. Mapping the core elements of specialized metadata standards to the schema.org schema is thus essential to enable this feature. The screenshots below show an example of an HTML page for a dataset published in a NADA catalog, with the underlying code. The structured metadata is used by Google to display this information as a formatted, "rich result" in Google Dataset Search.

<br>
**The HTML page as viewed by the catalog user** - The web browser will ignore the embedded structured metadata when the HTML page is displayed. What users will see is entirely controlled by the catalog application. 
<br>

<br>
<center>
![](./images/reDoc_html_view.JPG){width=80%}
</center>
<br>

<br>
**The HTML page code (abstract)** - The automatically-generated structured data can be seen in the HTML page code (or *page source*). This information is visible and processed by Google, Bing, and other search engine's web crawlers. Note that the structured data, although not "visible" to users, can be made accessible to them via API. Other data cataloguing applications may be able to ingest this information; the CKAN cataloguing tool for example makes use of metadata compliant with DCAT or schema.org. Making the structured data accessible is one way to improve the inter-operability of data catalogs.
<br>

<br>
<center>
![](./images/reDoc_html_code.JPG){width=80%}
</center>
<br>

<br>
**The result - Higher visibility/ranking in Google Dataset Search** - The websites catalog.ihsn.org and microdata.worldbank.org are NADA catalogs, which embed schema.org metadata. 
<br>

<br>
<center>
![](./images/reDoc_html_rank.JPG){width=80%}
</center>
<br>


## Use of controlled vocabularies

Metadata standards and schemas provide lists of elements with a description of the expected content to be captured in each element. For some elements, it may be appropriate to restrict the valid content to pre-selected options or "controlled vocabularies". A controlled vocabulary is a pre-defined list of values that can be accepted as valid content for some elements. For example. a metadata element "data type" should not be populated with free text, but should make use of a pre-defined taxonomy of data types. The use of controlled vocabularies (for selected metadata elements) will be particularly useful to implement search and filter features in data catalogs (see section 3.1.1 of this Guide), and to foster inter-operability of data catalogs.

:::quote
In library and information science, controlled vocabulary is a carefully selected list of words and phrases, which are used to tag units of information (document or work) so that they may be more easily retrieved by a search.[Wikipedia](https://en.wikipedia.org/wiki/Controlled_vocabulary)
:::

Controlled vocabularies can be specific to an agency, or be developed by a community of practice. For example, the list of countries and codes provided by the [ISO 3166](https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes) can be used as a controlled vocabulary for a metadata element `country` or `nation`; the [ISO 639](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) list of languages can be used as a controlled vocabulary for a metadata element `language`. Or the [CESSDA topics classification](https://vocabularies.cessda.eu/vocabulary/TopicClassification) can be used as a controlled vocabulary for the element `topics` found in most metadata schemas. When a controlled vocabulary is used in a metadata standard or schema, it is good practice to include an identification of its origin and version.  

Some recommended controlled vocabularies are included in the description of the ISO 19139 standard for geographic data and services (see chapter 6). Most standards and schemas we recommend also include a `topics` element. Annex 1 provides a description of the CESSDA topics classification. 

Ideally, controlled vocabulary will be developed in compliance with the [FAIR principles](https://www.go-fair.org/fair-principles/) for scientific data management and stewardship: **F**indability, **A**ccessibility, **I**nteroperability, and **R**euse.


## Use of tags 

All metadata standards and schemas described in this guide include a `tags` element, even when this element is not part of a standard. This element enables the implementation of filters (facets) in data cataloguing applications, in a flexible manner. The `tags` metadata element is repeatable (meaning that more than one tag can be attached to a dataset) and contains two sub-elements to capture a `tag` (word or phrase), and the `tag_group` (if any) it belongs to.

<center>
![](./images/reDoc_tags.JPG){width=100%}
</center>

To illustrate the use of tags, let's assume that a catalog contains datasets that are available freely, and others that are available for a fee. The catalog administrator may want to provide a filter (facet) in the user interface that would allow users to filter datasets based on their free or not free status. None of the metadata schemas we describe in the Guide contains an element specifically designed to indicate the "free" or "for a fee" nature of the data. But this information can be captured in a tag "*Free*" or "*For a fee*" that would be added to each dataset in the catalog, with a tag group that could be named "free_or_fee". In R, this would be done as follows (for a "Free" dataset):


```r
# ... ,
tags = list(
  list(tag = "Free", tag_group = "free_or_fee")
)
# ... 
```
    
In the NADA catalog, a facet titled "Free or for a fee" can then be created based on the information found in the `tags` element where `tag_group` = "free_or_fee".

<center>
![](./images/reDoc_tags_2.JPG){width=100%}
</center>


## Metadata augmentation

Detailed and complete metadata foster usability and discoverability of data. Augmentation of "enrichment" or "enhancement" of the metadata --which can apply to any metadata standard-- will therefore be beneficial. There are multiple ways metadata can be programmatically augmented. Metadata can be extracted from external sources or from the data themselves. This augmentation process often requires the use of  machine learning or artificial intelligence tools and methods.  

**Extraction from external sources**

Metadata can be augmented by tapping into external sources related to the data being documented. For example, in a catalog of documents published in peer-reviewed journals, the [Scimago Journal Rank (SJR)](https://www.scimagojr.com/) indicator could be extracted and added as an additional metadata element for each document. This information can then be used by the catalog's search engine to rank query results, by "boosting" the rank of documents published in prestigious journals. Information on the popularity of a dataset (for example, measured by the number of downloads), and information on the uses and users of the dataset (for example, by maintaining a catalog of citations of the dataset) can also contribute to enriching the metadata. Some of this information may be stored in the structured metadata, other (like the number of downloads) may be dynamically extracted from a cataloguing application.

**Extraction from the data** 

Metadata can be extracted from the data themselves. What metadata can be extracted will be specific to each data type. Examples of metadata augmentation is provided in chapters 5 to 13. We mention a few below.

   - For microdata: variable-level statistics (range of values, number of valid/missing cases, frequencies for categorical variables, summary statistics like means or standard deviations for continuous variables) can be extracted and stored as metadata. Topics and variable groups can be extracted from the data dictionary using AI-based tools.

   - For documents: information such as the country counts (how many times each country is mentioned) can be extracted automatically to fill out the metadata element related to geographic coverage. Natural language processing (NLP) models can be applied to automatically extract keywords or topics (e.g., using a Latent Dirichlet Allocation - LDA - topic model). Classification models can be applied to categorize documents by type. 
   
**Embeddings and semantic discovery**

Previous sections of the chapter showed the value of rich and structured metadata to improve data usability and discoverability. Comprehensive and structured metadata are required to build and develop advanced and optimized <u>lexical</u> search engines (i.e. search engines that return results based on a matching of terms found in a query and in an inverted index). The richness of the metadata guarantees that the search engine will have all necessary "raw material" to identify datasets of interest. The metadata structure allows catalog administrators to tune their search engine (provided they use advanced solutions like Solr or ElasticSearch) to return and rank results in the most relevant manner. But this leaves one issue unsolved: the dependency on keyword matching. A user interested in datasets related to *malnutrition* for example will not find the indicators on *Prevalence of stunting* and *Prevalence of wasting* that the catalog may contain, unless the keyword "malnutrition" was included in these indicators' metadata. Smarter search engines will be able to "understand" users intent, and identify relevant data based not only on a keyword matching process, but also on the **semantic closeness** between a query submitted by thea user and the metadata available in the database. The combination of rich metadata and natural language processing (NLP) models can solve this issue, by enabling semantic searchability in data catalogs.

To enable a semantic search engine (or a recommender system), we need a way to "quantify" the semantic content of a query submitted by the user and the semantic content the metadata associated with a dataset, and to measure the closeness between them. This "quantitative" representation of semantic content can be generated in the form of numeric vectors called **embeddings**. "Word embedding is a term used for the representation of words for text analysis, typically in the form of a real-valued vector that encodes the meaning of the word such that the words that are closer in the vector space are expected to be similar in meaning." (Jurafsky, Daniel; H. James, Martin (2000)). These vectors will typically have a large dimension, with a length of 100 or more. They can be generated for a word, a phrase, or a longer text such as a paragraph or a full document. They are calculated using models like word2vec (Mikolov et al., 2013) or other. Training such models require a large corpus of hundreds of thousands or millions of documents. Pre-trained models and APIs are available that allow data catalog curators to generate embeddings for their metadata and, in real time, for queries submitted by users.

Practically, embeddings are used as follows: metadata (or part of the metadata) associated with a dataset are converted into a numeric vector using a pre-trained embedding model. These embeddings are stored in a database. When a user submits a search query (which can be a term, a phrase, or even a document), the query is analyzed and enhanced (stop words are removed, spelling errors may be fixed, language detection and automatic translation may be applied, and more), then transformed into a vector using the same pre-trained model that was used to generate the metadata vectors. The metadata vectors that have the shortest distance (typically the cosine distance) with the query vector will be identified. The search engine will then return a sorted list of datasets having the highest semantic similarity with the query, or the distance between vectors will be used in combination with other criteria to rank and return results to the user. The fast identification of the closest vectors requires a specialized and optimized tool like the open source [Milvus](https://milvus.io/) application.
   
   - For geospatial data: bounding boxes (i.e. the *extent* of the data) can be derived from the data files. 
   
   - For photos taken by digital cameras: metadata such as the date and time the photo was taken and possibly the geographic location can be extracted from the EXIF metadata generated by digital cameras and stored in the image file. Also, machine learning models allow image labeling, face detection, text detection and recognition to be applied at low cost (using commercial solutions like [Google Vision](https://cloud.google.com/vision) or [Amazon Rekognition](https://aws.amazon.com/rekognition/) among others). 
   
   - For videos and audio files, machine learning models of speech-to-text API solutions can be used to automatically generate transcripts (see for example [Amazon Transcribe](https://aws.amazon.com/transcribe/), [Google Cloud Speech-to-Text](https://cloud.google.com/speech-to-text), [Microsoft Azure Speech to Text](https://azure.microsoft.com/en-us/services/cognitive-services/speech-to-text/), or [rev.ai](https://www.rev.ai/)). The content of the transcripts can then be indexed in search engines, making the content of video and audio files more discoverable. 
   
   - For programs and scripts: a parsing of the commands used in the script may be used to derive information on the methods applied.

[^1] See Omar Benjelloun, Shiyu Chen, Natasha Noy, 2020, *Google Dataset Search by the Numbers*, https://doi.org/10.48550/arXiv.2006.06894
