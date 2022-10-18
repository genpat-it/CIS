# COHESIVE Information System

## A data platform to facilitate risk‐analysis and outbreak control

The OHEJP COHESIVE project aims at improving efficiency on surveillance, risk assessment and outbreak management through a One-Health approach at Member State level. The achievement of such an objective would require that each Member State the integration of pathogen data from the human, veterinary and food sectors in each Member State.

Below is a series of links to project documents shared through general-purpose open repository Zenodo.

#### D-JIP2-4.1.1 Implemented database

The CIS (Cohesive Information System) is basically a database with WEB interface based on the opensource CMDBUILD Project. CMDBuild is an open source web enterprise environment used to configure custom applications and to manage databases of items.

Data from different sources (Metadata from Member State, WGS Analysis and  every type of input relevant for a Member State) are collected into a Database (COHESIVE Cache) where they are subjected to a process of transformation and sanitation (cleaning) in order to make them homogeneous. Subsequently these data are subjected to a process of validation and only at this point they are ready to be transferred to the PostgresSQL database of the CIS.

[https://zenodo.org/record/5785904#.YbskXy5KgYM](https://zenodo.org/record/5785904#.YbskXy5KgYM)

#### COHESIVE Information System (CIS) Virtual Machine (COHESIVE)

Link for the image of the Virtual Machine produced.

[https://www.zenodo.org/record/3342485#.Y06iPS0QPtt](https://www.zenodo.org/record/3342485#.Y06iPS0QPtt)

#### COHESIVE Information System (CIS) Virtual Machine Technical Specifications (COHESIVE)

We have installed the CIS system in a virtual machine so that each member state can import it into their own systems and use the application. The virtual machine contains all the components system needed to the CIS system, such as the web application and the database.

In the following document, an explaination on how to import the virtual machine shared in Zenodo website into the VirtualBox and launch the application to use the CIS system.

[https://www.zenodo.org/record/3354124#.Y06i3S0QPtt](https://www.zenodo.org/record/3354124#.Y06i3S0QPtt)

#### Milestone M JIP2-4.1: Initial workshop Workpackage 4.1 (COHESIVE)

COHESIVE Initial Workshop November 26 & 27 2018

[https://www.zenodo.org/record/3457753#.Y06jDi0QPtt](https://www.zenodo.org/record/3457753#.Y06jDi0QPtt)

#### D-JIP2-4.1.2 Description of the links and the linked databases (COHESIVE)

This deliverable is aimed at connecting the three databases needed by the project: 
- a DB for WGS data consistent with COMPARE standards, 
- a DB for the metadata of the samples included in the WGS database, 
- a DB for the data collected by classical epidemiology investigations (case-control studies). 

In that way metadata is properly connected to the relevant WGS information, and data collected on patients without a genetic typing of their pathogens may be, whenever possible, linked to the relevant cluster of pathogen genomes.

- Italy has chosen to investigate the pathogen “Listeria monocytogenes”.
- Norway has chosen to investigate the pathogen “Listeria monocytogenes”.
- The Netherlands has chosen to investigate the pathogens “Listeria monocytogenes” and “Hepatitis E”.

[https://zenodo.org/record/5785745#.Y06jVy0QPtt](https://zenodo.org/record/5785745#.Y06jVy0QPtt)

#### D-JIP2-4.1.3 Databases containing the country data (COHESIVE)

In this deliverable we have filled the three DB of this project (WGS, metadata and classicalepidemiology) with the data available from three participating countries, such as:
- Italy;
- Norway;
- The Netherlands.

For the collection of metadata we have sent to all Member States a template to be filled with the metadata of interest in order to identify the minimal set of metadata needed in an outbreak. Italy and The Netherlands provided information to fill the relative COHESIVE Information System (CIS). Norway activity is still on going.

[https://zenodo.org/record/5785758#.Y06jpi0QPtt](https://zenodo.org/record/5785758#.Y06jpi0QPtt)

#### M‐A2.COHESIVE.4.7 - Databases containing the country data (COHESIVE)

In this milestone we have filled the three DB of this project (WGS, metadata and classicalepidemiology) with the data available from three participating countries, such as:
<!--
- Italy, [https://cohesive.izs.it/cis_italy/](https://cohesive.izs.it/cis_italy/);
- Norway, [https://cohesive.izs.it/cis_norway/](https://cohesive.izs.it/cis_norway/);
- The Netherlands (https://cohesive.izs.it/cis_holland/).
-->

[https://www.zenodo.org/record/4501287#.Y06kVi0QPtt](https://www.zenodo.org/record/4501287#.Y06kVi0QPtt)

#### Refinement of the COHESIVE Information System towards a unified ontology of food terms for the public health organizations (COHESIVE)

**Background**
The task 4.1 of the One Health European joint programme (OHEJP) “One Health Structure In Europe” (COHESIVE) focuses on integrating pathogen information from public health, animal health and food safety surveillance at Member State level. Considered information are metadata associated to each sample (i.e. isolation date, origin, matrix) and whole genome sequencing (WGS) data from official laboratories (e.g. next generation sequencing data and bioinformatics-based analytical outcomes).

**Methods**
A WEB-based platform called the COHESIVE Information System (CIS) has been created with separate instances for three Member States, in order to provide a proof of concept showing the advantages for surveillance and investigation of outbreaks at the genomic scale, considering food as a source of human pathogens. Currently, a CIS Version 2 (CISv2) is under development to integrate a unified food ontology at Member State level, taking into account as a first step organizations from Italy, Norway and The Netherlands: countries involved in the feasibility study foreseen in the project. More precisely, the last developments focused on the harmonization of the foodborn disease biosample contextual data collected over the past few decades (i.e. contextual metadata of foodborne samples sent in by labs for sequencing) based on the rule-based text mining tool LexMapr, and the implementation of the FoodOn ontology into the CIS based on the graph-database Neo4j to allow future records of harmonized food terms in the CISv2.

**Results**
The successful harmonization of the past food terms and implementation of the FoodOn ontology into the CIS were mandatory steps allowing food ontology harmonization between organizations and improvement of queries from theCISv2 based on relational- and graph-databases.

[https://www.zenodo.org/record/5482422#.Y06kqC0QPtt](https://www.zenodo.org/record/5482422#.Y06kqC0QPtt)

#### D-JIP2-4.1.4 Description of the pipelines implemented to feed the analysis tools with the data stored in the three databases of this project (COHESIVE)

The purpose of this deliverable is the design and implementation of common pipelines to be available in CIS and related three instances for involved Member States. 

The idea was not to realize additional bioinformatic tools, but to combine the most common available tools for the analyses of pathogens involved in the pilots. 
For this purpose, partial information was gathered from involved Member States. Additional specifications has been taken from a deliverable of OHEJP ORION project: “The One Health Sequencing for Surveillance Handbook” - [https://oh-sfs-handbook.readthedocs.io/](https://oh-sfs-handbook.readthedocs.io/)

Laveraging on those information, we assembled a pipeline able to analyze Bacterias strains in general, and Listeria monocytogenes in particular. The latter because it was the pathogen chosen by the pilots.
The pipeline is named NgsManager (avaliable at [https://github.com/genpat-it/ngsmanager](https://github.com/genpat-it/ngsmanager)) 

Additionally, NgsManager is also able to manage SARS-CoV-2 samples.

[https://zenodo.org/record/5785798#.Y06lSC0QPtt](https://zenodo.org/record/5785798#.Y06lSC0QPtt)

#### M_A2.COHESIVE.4.9 Availability of the pipelines from the databases to the analysis tools (COHESIVE)

The purpose of this milestone is the design and implementation of common pipelines to be available in CIS and related three instances for involved Member States. The idea was not to realize additional bioinformatic tools, but to combine the most common available tools for the analyses of pathogens involved in the pilots.

Laveraging on those information, we assembled a pipeline able to analyze Bacterias strains in general, and Listeria monocytogenes in particular. The latter because it was the pathogen chosen by the pilots. The pipeline is named NgsManager (avaliable at [https://github.com/genpat-it/ngsmanager](https://github.com/genpat-it/ngsmanager)).

[https://www.zenodo.org/record/5764300#.YbnVfC5KgYM](https://www.zenodo.org/record/5764300#.YbnVfC5KgYM)

## Repo under construction
