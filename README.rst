Untargeted Metabolomics Pipeline 
================================

:Authors: Lin An; Difei Wang, Ph.D.
:Emails: difei.wang AT georgetown.edu or wang.difei AT yahoo.com or difei.wang AT nih.gov

Description
===========
This pipeline was developed by Mr. Lin An who worked with me as an intern at ICBI, Georgetown University from 2013 to 2014. He used this pipeline to process Duchenne muscular dystrophy samples from the National Children's Hospital and space shuttle samples from the US Military.

Requirement
===========

  - Windows, MacOS and Linux
  - Python, R, MySQL
  - Package: Python (MySQLdb, csv), R (XCMS, CAMERA, Multtest)

Running steps
=============
- Import hmdbchem1.sql to local mysql database
- Set up raw data path in Metaanalysis.R
- Set up parameters for analysis
- Run Metaanalysis.R
- Filter peak results by fold change and p-value
- Save filtered results in a new csv file
- Run annotation.py with the filtered results
- Retrieve annotation data from Metlin database
- Integrate annotation data

