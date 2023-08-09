---
title: Governance with Purview
menutitle: Governance with Purview
author: 
  - fcortella
weight: 03
chapter: false
date: 2023-07-31
draft: false
alwaysopen: false
featured: true
summary: "Fabric"
shortlink: aka.ms/beluxpartnertech/data/cloud-scale-analytics
caption: /images/solutionareas/business-decisions.png
---


Microsoft Purview is a family of data governance, risk, and compliance solutions that can help your organization govern, protect, and manage your entire data estate. The solution portfolio can be divided into two different categories:
- Unified Data Governance (pay-per-use cloud consumption model, previously named Azure Purview)
- Risk and compliance (commercialized via licenses, previously named Microsoft 365 Compliance)
  
**As in this hub we are covering Data & AI, we will focus only on the the Unified Data Governance part of Microsoft Purview**, which provides a solution to help manage and govern your on-premises, multicloud, and software as a service (SaaS) data. It helps you to:

- Create a holistic, up-to-date map of your data landscape with automated data discovery, sensitive data classification, and end-to-end data lineage
- Enable data consumers to access valuable, trustworthy data
- Gain insights into the management and quality of sensitive data across your entire data estate
- Enables at-scale access provisioning
- Share data in place without having to make duplications

We invite you to learn about Purview data governance solutions and its components: Data Map, Data Catalog app, Data Estate Insights app, Data Sharing app, and Data Policy app. You can find all the relevant documentation and trainings [<u>here</u>](https://learn.microsoft.com/en-us/purview/governance-home).


## Engagements break-down

As partner, it is good to be aware that (almost) all the customer projects have this life-cycle:

**Stage 1 – Azure Purview**
Identify sources
Identify domains, define collection strategy (granularity)
Define first use case(s)
Determine 'just-enough' governance
Define governance requirements and success criteria
List out data ownership roles, data stewardship roles, application ownership roles, etc.

**Stage 2 – Curate technical metadata**
Deploy Purview
Create collection structure
Register first data sources
Configure scan rule sets
Validate, update filters and scan rule sets, iterate.
Create managed attributes for additional technical metadata information

**Stage 3 – Curate business metadata**
Define glossary structure, e.g., multi-glossary or parent/child structures
Import content from other sources
Setup term templates
Setup business term workflows
Define and develop linkage criteria

**Stage 4 – Lineage**
Scan integration services
Develop scripts or functions for utilizing APIs / SDKs
Curate missing lineage using manual lineage panes

**Stage 5 – Advance**
Implement business metamodel
Setup classification and sensitivity label schemes
Configure insights overviews
Add self-service data access and data use policies
Add additional features

## Advanced material

Finally, we invite you to explore the following resources for integration and customization:
- [<u>GitHub - wjohnson/pyapacheatlas: A python package to help work with the apache atlas REST APIs<u>](https://github.com/wjohnson/pyapacheatlas)
- [<u>GitHub - tayganr/purviewcli: Azure Purview CLI<u>](https://github.com/tayganr/purviewcli)
- [<u>Official Python SDK: Azure SDK for Python (All) | Purview<u>](https://azure.github.io/azure-sdk/releases/latest/all/python.html)
- Registration of custom sources and lineage via API: [<u>Use Azure Purview’s REST APIs for creating custom lineage<u>](https://piethein.medium.com/use-azure-purviews-rest-apis-for-creating-custom-lineage-ad8efacc6230)
- Integrate Azure Synapse Analytics and Azure Purview together to build a framework for intelligently processing data: [<u>Modern Data Pipelines with Azure Synapse Analytics and Azure Purview<u>](https://piethein.medium.com/modern-data-pipelines-with-azure-synapse-analytics-and-azure-purview-fe752d874c67)
- Programmatically monitor for metadata changes in real-time, allowing you to enrich your user experience by also integrating with other services: [<u>Process events from Azure Purview’s Atlas Kafka topics via Event Hubs and NodeJS<u>](https://piethein.medium.com/process-events-from-azure-purviews-atlas-kafka-topics-via-event-hubs-and-nodejs-cfcbe044bb2c)
- Databricks Solution Accelerator: <u>https://github.com/microsoft/Purview-ADB-Lineage-Solution-Accelerator<u>. Uses OpenLineage connector that will transfer lineage metadata from Spark operations in Azure Databricks to Microsoft Purview, allowing you to see a table-level lineage graph as demonstrated above.
- Metadata-driven processing framework: <u>https://piethein.medium.com/designing-a-metadata-driven-processing-framework-for-azure-synapse-and-azure-purview-33121a63ebc0.<u> Uses a SQL Server metadata database for iteratively executing Notebooks. The pipeline metadata will be used for transferring lineage to Purview.
- <u>https://github.com/pietheinstrengholt/Purview-Bulk-Collection-Mover<u>
