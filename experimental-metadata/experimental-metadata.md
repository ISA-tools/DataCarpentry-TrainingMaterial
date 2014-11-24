# Experimental Data Carpentry #
## Managing life science experimental metadata in tables ##

Authors: <br>
Contributors:

## Experimental Data ##

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

On the other hand, creating the metadata can be time-consuming. So, it is important to provide sufficient information to understand en enable re-use of the dataset, but at the same time striking a balance between the depth and breadth of the metadata provided.

Several communities in the different domains have worked on developing a variety of metadata standards focusing on specifying the content to be reported, the formats to be used and common terminologies for each of domains. By agreeing on what to report

In the next section, we will explore the different types of community-based metadata standards, providing examples for life science domains.

## Metadata Standards ##

* Minimum Information Checklists: identify the same core, essential information to report about a particular type of experiment 
* Exchange Formats: allow information to flow from one system to another (enabling syntactic interoperability)
* Terminologies: emphasise on using the same term for referring to the same 'thing' in multiple systems (enabling semantic interoperability)

Compliance with the standards is challenging. We will next present an example infrascture whose design aim was to:

* achieve a common, structured representation of diverse bioscience experiments and transcending specific domains
* facilitating compliance with the specific community guidelines and standards

### Semantic Annotation ###


