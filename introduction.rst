Introduction
============
    The purpose of this document is to specify a set of requirements for the OMG project, which means "Oh, my genes", a web application used to identify differences in gene expression.


Purpose
-------
    A gene expression file containing two cell samples is presented. The main purpose is to help biologists analyze their experimental data. 


Overview
--------
    The web application has a simple interface with a single button [Upload and GO]. Our scientists upload a plain text file containing gene expression levels from two samples, representing two experimental conditions. Accepting the file, the software will return a table of differentially expressed genes and a scatter plot of these genes whose X-axis is control and Y-axis is treatment. If an invalid gene expression is given, the web application returns a page informing the user to provide the correct format.


User Characteristics
--------------------
    *   **Client User:** A biologist who studies gene expression.
    *   **Site Maintainer:** Technicians with flask and Python basics maintain the site.

Terminologies & Abbreviations Explaination
------------------------------------------
    For the purpose of detailing the project and specifying the requirements, this section aims to explain a number of terms and abbreviations in order to better understand the content of the project.

Terminologies
~~~~~~~~~~~~~
================================  ==================================================================
  Term                                                       Definition
================================  ==================================================================
Control sample                    A cell samples prepared under normal conditions
Treatment sample                  A cell samples treated with specific chemicals, or cells whose genes have been altered.
Up-regulation                     A gene is said to be up-regulated if it has higher expression in treatment than in control.
Differentially expressed genes    The genes which have significantly different expression levels between two samples. 

Abbreviations
~~~~~~~~~~~~~
    
    *   *OMG* - means Oh My Genes.
    *   *logFC* - log fold change of gene expression. Log2 (T/C), where T is the gene expression level from a treatment sample, and C is the gene expression level from a control sample
