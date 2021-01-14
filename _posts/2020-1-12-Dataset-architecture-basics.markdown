---
layout: post
title: "Dataset architecture basics"
date:  2021-1-12
category: data basics

---

In bioinformatic research, databases place a vital role in analysis efforts. Whether it’s sequence data, patient data, 
taxonomic IDs--all of this information is organized and structured in some form of a database, data pool, data lake, long text files, JSON, XML, and so on. 
What is the difference between all these data architectures? A little thing called structure.

![Photo by Fiona Smallwood on Unsplash](https://github.com/kbeckenrode/kbeckenrode.github.io/blob/main/assets/images/fiona-smallwood-6CszxGveP8U-unsplash%20(1).jpg)

*Tidy life, tidy data? Photo by Fiona Smallwood on Unsplash*


Data is made of values: either number (*quantitative*) and/or strings (*qualitative*), and values can be arranged in few typical ways. 
Let’s define the 3 different types of data organization:

**Structured** means data is organized in a table and a relationship exists between rows and columns. Structured data requires a data model, 
which is a set of consistent rules for storage, arrangement, and access. The most common examples of structured data are Excel and SQL spreadsheets. 

Data architecture jargon for “structured data”: [database](https://en.wikipedia.org/wiki/Database), [data warehouse](https://en.wikipedia.org/wiki/Data_warehouse)

**Unstructured** data refers to information without a data model--or in other words: does not fit into a spreadsheet. 
Unstructured data can still have some structure, but if it’s not physically organized in a way to help perform analytics, then it is called unstructured. 
The most common examples of unstructured data are pictures, video, and log files. Even social media posts. 

Data architecture jargon for “unstructured data”: [data lake](https://en.wikipedia.org/wiki/Data_lake), [data pool](https://liliendahl.com/2018/04/21/data-pool-vs-data-lake/)

**Semi-structured** data does not conform to either structured or unstructured architectures, but have qualities of both. While having some structures,
like separated by commas, or other elements to note organization. The most common examples of semi-structured data are [XML](https://en.wikipedia.org/wiki/XML) 
(eXtensible markup language) and [JSON](https://en.wikipedia.org/wiki/JSON) (JavaScript Object Notation). Both of these formats are human-readable and machine-readable to store data arrays. 

As a bench scientist, I took data architecture and management for granted. When I started creating my own database, I quickly appreciated that 
database creation demands respect and careful consideration. Here are some basic universal principles for database creation. 

# A few do’s and don’t’s for database architecture 
1. A standard for [tidy](https://tidyr.tidyverse.org/) data is

    a. Every column is variable.
    
    b. Every row is an observation.
    
    c. Every cell is a single value. 
  
2. Use domain lanuugage standards. Meaning, don't invent new terms to describe well-established words. For establishing a standard vocubulary, consider using an [ontology](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3230227/).

3. Making a database is a process. Formatting the data will only illuminate new problems, so you reformat and find new problems, and so on. Be patient.

4. Understand how the database will be used. By who? For what application? What kind of analysis will users perform?

5. Zero and missing values are valuable. If you have [large sparse data](https://cran.r-project.org/web/packages/SparseM/vignettes/SparseM.pdf), you may need to develop a different plan for storage and processing. 

6. Remember, what you put into your database is what will come out: diamonds in, diamonds out;  garbage in, garbage out.

7. If you are not using version control, make sure to create backups.

8. Don’t forget to document your process. The notes on how you created the database will be vital for users and anyone needing to work on the dataset.

If you are using R, [tidyr helps create clean and clear datasets](https://tidyr.tidyverse.org/). For more information on 
[Tidy Data](https://cran.r-project.org/web/packages/tidyr/vignettes/tidy-data.html), especially to read more about the #1 rule above, follow the link 
[Here is the full Tidy data paper](https://vita.had.co.nz/papers/tidy-data.html).

