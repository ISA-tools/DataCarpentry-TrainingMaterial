# Experimental Data Carpentry #
## Managing life science experimental metadata in tables ##

Authors: <br>
Contributors:

Sculpting data, i.e. generating data and annotating data, involves a wide set of skills ranging from knowledge about the data in the specific domain being considered, plus general expertise on data management, enabling the storage, interpretation, preservation and re-use of data.

This tutorial will explore some of the concepts, required skills and available software tools useful for managing the data and metadata --- or data about the data --- maintained in tables, i.e. in spreadsheet programs. 

## Experimental Data ##

The last decade has seen a massive increase on the biological data being generated. Considering DNA sequencing technologies as an example, there has been an impressive improvement in instruments capacity during the last ten years, when moving from Sanger-based capillary sequencing methods to next generation, massively parallel sequencing technologies (see Mardis 2011). In addition to the technological enhancements, the sequencing costs have been dropping (see http://www.genome.gov/sequencingcosts/). 

## Experimental Metadata ##

The data on their own is not enough to understand what the data are about and how they were generated. It is important to record information about the data generation process, not only for sharing the data with other people, but also for being able to understand one's own data in the future.

Let's see some examples on how NOT to report experimental information.

Imagine you found a folder entitled ```LS1_C2_LD_TP2_P1``` containing a file ```file1-fastq.gz```. So, what data does the file contains?

As the file extension is ```gz```, we can figure out that is a compressed file following the [GZip file format](http://en.wikipedia.org/wiki/Gzip#File_format). As it is a ```fastq``` file, we can assume it contains sequence information following the [FASTQ format](http://en.wikipedia.org/wiki/FASTQ_format).

But what is the sample this sequence data comes from?

We can guess that the folder name follows some coding system, but which one? It would be necessary to have that information spelled out.

The table below shows an example of what the data creator could have meant:

        Code  | Meaning
------------- | -------------
         LS1  | liver sample 1
          C2  | compound 2
          LD  | low dose
         TP2  | time point 2
          P1  | protocol 1

To make the data understandable, re-usable and, in principle, reproducible, it is crucial to provide metadata --- or data about the data --- including the experimental steps followed to produce the data, the characteristics of the samples, the protocols applied, the transformations applied and so on.

On the other hand, creating the metadata can be time-consuming. So, it is important to provide sufficient information to understand en enable re-use of the dataset, but at the same time striking a balance between sufficiency and practicability, by exploring the depth and breadth of the metadata provided.

Several communities in the different domains have worked on developing a variety of metadata standards focusing on specifying the content to be reported, the formats to be used and common terminologies for each of domains. By agreeing on what to report

In the next section, we will explore the different types of community-based metadata standards, providing examples for life science domains.

## Metadata Standards ##

Community-developed metadata standards can be classified into three categories:

* **Minimum Information Checklists**: these are guidelines to identify the core or essential information to report about a particular type of experiment 
* **Exchange Formats**: formats that allow information to flow from one system to another (enabling syntactic interoperability)
* **Terminologies**: emphasise on using the same term for referring to the same 'thing' in multiple systems (enabling semantic interoperability); these terminologies could include a wide-range of vocabularies, from taxonomies to more formal ontologies.

Let's now explore each of these categories, highlighting some examples of each.





Compliance with the standards is challenging. We will next present an example infrascture whose design aim was to:

* achieve a common, structured representation of diverse bioscience experiments and transcending specific domains
* facilitating compliance with the specific community guidelines and standards

### Semantic Annotation ###


