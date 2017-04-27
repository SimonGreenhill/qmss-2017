
# Data curation with git and GitHub

We already learned about the advantages of using git and GitHub to collaborate on research projects.
A special kind of research project is the curation of a dataset. For research data to be amenable for
curation via git means:

- it should consist of a collection of text files
- individual text files should not be too big, and have a line-based format

It turns out that quite a few datasets important to us can be modelled in this way, and CSV - everyone's 
favorite format for tabular data - is gaining popularity every day:

- Glottolog:
  - Bibliographic information is stored as set of BibTeX files
  - Language information is stored as one INI file per language
  - directory tree models the language classification

- D-PLACE
- Concepticon
- Gelato

For relational data, though, this approach sacrifices a built-in mechanism to enforce referential integrity
(which relational databases provide). But this can be alleviated using scripts to check data consistency
(and using the GitHub platform these checks could be run automatically).

See also https://github.com/clld/lanclid2/blob/master/presentations/forkel.pdf