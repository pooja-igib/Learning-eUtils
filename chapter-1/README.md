# Chapter-1 | Searching a database
[link](https://www.ncbi.nlm.nih.gov/books/NBK25500/#chapter1.Searching_a_Database)

Base URL for all E-utility calls:
*https://eutils.ncbi.nlm.nih.gov/entrez/eutils/*

## Basic Searching ##

*esearch.fcgi?db=<database>&term=<query>*

Input: Entrez database (&db); Any Entrez text query (&term)

Output: List of UIDs matching the Entrez query

## Storing Search Results ##

*esearch.fcgi?db=<database>&term=<query>&usehistory=y*

Input: Any Entrez text query (&term); Entrez database (&db); &usehistory=y

Output: Web environment (&WebEnv) and query key (&query_key) parameters specifying the location on the Entrez history server of the list of UIDs matching the Entrez query

## Searching PubMed with Citation Data ##

ecitmatch.cgi?db=pubmed&rettype=xml&bdata=<citations>

Input: List of citation strings separated by a carriage return (%0D), where each citation string has the following format:
journal_title|year|volume|first_page|author_name|your_key|

Output: A list of citation strings with the corresponding PubMed ID (PMID) appended.



