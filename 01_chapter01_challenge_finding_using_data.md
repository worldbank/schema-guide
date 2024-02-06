---
output: html_document
---

# (PART) RATIONALE AND OBJECTIVES  {-}

# The challenge of finding, accessing, and using data {#chapter01}

Many organizations share data online, making numerous and diverse datasets accessible to researchers and analysts. However, a significant challenge arises in practically finding, accessing, and utilizing this wealth of data. Navigating through the vast and continually expanding pool of data sources available online often demands significant time and effort, without a guaranteed identification of datasets that best align with the researcher's needs. Complexities arise from issues such as insufficient metadata, limitations in data discovery tools, and the restricted visibility of valuable data repositories. Addressing technical hurdles related to data discoverability, accessibility, and usability is crucial for improving data sharing policies and optimizing the utility of collected data. The following sections will provide a detailed exploration of these challenges.  

## Finding data

Researchers and data users employ a variety of strategies to pinpoint and procure existing datasets. While some leverage personal networks or academic publications to identify datasets of interest, this approach may result in the utilization of readily available yet suboptimal information. Conversely, many data users resort to utilizing general search engines or specialized data catalogs in their pursuit of pertinent and high-quality data resources.

Prominent internet search engines showcase significant capabilities in locating and ranking pertinent online resources. The algorithms behind these search engines integrate both lexical and semantic functionalities. Straightforward data queries, such as searching for *population of India 2023*, yield instant answers (though not always from the most authoritative source). Less specific queries, like searching for *malnutrition in Yemen*, may not provide a direct answer but offer sufficient information and links to useful resources. Generative artificial intelligence is enhancing these search engines' ability to engage with users using natural language, suitable for addressing simple queries, albeit with the potential for errors and inaccuracies. However, internet search engines are not optimized to identify the most relevant data when user requirements cannot be expressed as a straightforward query.

Specialized online data catalogs or data libraries managed by national or international organizations, as well as academic data centers, provide an alternative avenue for researchers in search of valuable data. These catalogs typically offer lexical search capabilities (keyword-based search), althoughnot always optimally implemented. Most notably, the absence of semantic search capabilities, coupled with limitations in the underlying metadata, hinders their effectiveness as data recommender systems. However, with the rapid evolution of technology and the accessibility of robust open-source solutions, it is feasible to significantly enhance the search performance of specialized data catalogs, thereby transforming them into efficient data recommender systems. This transformation necessitates the adoption of superior technology, coupled with the integration of high-quality, comprehensive, and well-structured metadata. Metadata, serving as a detailed description of datasets, is the foundation upon which search engines rely to proficiently identify and locate data of interest.

:::quote
Metadata is structured information that describes, explains, locates, or otherwise makes it easier to retrieve, use, or manage an information resource. Metadata is often called data about data or information about information. (Source: National Information Standards Organization, 2004)

Good metadata enables you to understand, use, and share your own data now and in the future and helps other researchers discover, access, use, repurpose, and cite your data in the long term. It also facilitates long-term archival preservation of the data. (Source: [Harvard Medical School](https://datamanagement.hms.harvard.edu/collect-analyze/documentation-metadata))
:::

Metadata are not only needed to enable the data discovery systems. They are also required to allow users to assess the relevance, or fitness-for-purpose, of a dataset. Metadata is the first element that data users examine to assess whether the data align with their requirements. Acquiring a dataset can be time-consuming and occasionally costly activity. Users should be provided with the necessary information to assess the relevance of a dataset prior to acquiring it. 

## Accessing data

Gaining access to data presents a multifaceted challenge that encompasses legal, ethical, and practical considerations. To ensure that data access is not only lawful and ethical but also efficient, both data providers and users must adhere to specific principles and practices:

- **Legal framework**: Data providers must affirm their legal rights to share the data and articulate clear usage rights for data users. Data users must comprehend how they can employ the data, whether for research, commercial purposes, or other applications, strictly adhering to the specified terms of use.
- **Privacy and ethical standards**: Data access must align with data privacy laws and ethical standards, especially concerning sensitive or personally identifiable information. Handling such data requires utmost care to safeguard individuals' privacy.
- **Comprehensive metadata**: Data providers play a crucial role in furnishing comprehensive metadata that offers context and a thorough understanding of the data. This metadata should encompass details about the data's provenance, including its history, transformations, and processing steps. This understanding is indispensable for accurate and responsible analysis.
- **User-friendly formats**: Data should be made available in user-friendly formats, including non-proprietary formats, compatible with common data analysis tools.
- **Convenient accessibility**: The modes of access should cater to various user preferences and capacities. This may involve offering downloadable data files, providing access through web-based tools, and supporting data streaming. Access to data via API (Application Programming Interface) empowers users to retrieve and manipulate data programmatically, seamlessly integrating them into their research workflows and applications.

By embracing these principles, the data community can navigate the challenges of accessing data, fostering a framework that ensures legality, ethics, efficiency, convenience, and relevance in data usage.

## Using data

Navigating data goes beyond mere discovery; it entails acquiring all essential information for a thorough comprehension of the data and fostering responsible and apt usage. Consider a seemingly straightforward indicator label, such as the unemployment rate — it could mask notable variations across countries, sources, and timeframes. The global guidelines for defining and calculating the unemployment rate have evolved, and the questionnaires and methodologies in national labor force surveys lack complete standardization. Therefore, comprehensive metadata should accompany data publications to provide clarity and context.

:::quote
The scope and meaning of labor statistics, in general, are determined by their source and methodology, which holds true for the unemployment rate. To interpret the data accurately, it is crucial to understand what the data convey, how they were collected and constructed, and to have information on the relevant metadata. The design and characteristics of the data source, typically a labor force survey or a similar household survey for the unemployment rate, especially in terms of definitions and concepts used, geographical and age coverage, and reference periods, have significant implications for the resulting data. Taking these aspects into account is essential when analyzing the statistics. Additionally, it is crucial to seek information on any methodological changes and breaks in series to assess their impact on trend analysis and to keep in mind methodological differences across countries when conducting cross-country studies. (From Quick guide on interpreting the unemployment rate, International Labour Office – Geneva: ILO, 2019, ISBN: 978-92-2-133323-4 (web pdf)).
:::

Whenever feasible and relevant, reproducible or replicable scripts used to process, generate, or analyze data should be published alongside the data. They add transparency and credibility to the data product, and can be highly valuable to researchers aiming to expand the scope of prior data analysis or reuse portions of the code. Chapter 12 of the Guide describes a specific metadata schema tailored for documenting research projects and scripts. 
