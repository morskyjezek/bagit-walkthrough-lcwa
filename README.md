# Demonstrating BagIt Concept and Tools

This repository holds materials for use in learning digital curation tools and concepts from archival and library perspectives. Specifically, this repository explains the **BagIt** specification (IETF RFC 8493) and associated, Python-based tools; these concepts and tools are demonstrated using sample files from the Library of Congress Web Archvies (LCWA). This short demonstration lesson was created as part of work on a larger set of lessons that outlines additional digital curation and preservation actions associated with all elements of the digital curation lifecycle.

## Lesson Concept: Demonstrate BagIt Structure and Creation Tools

This repository explains and situates the BagIt file packaging specification,
outlines the elements of file packages created according to the BagIt structure
("bags"), and then demonstrates how to create, assess, and maintain BagIt-conformant
bags using Python-based tools.

The goal is to demonstrate how computational tools (in this case, Python,
Jupyter notebooks, and Git) can be used to create file packages that can be
reliably transmitted to a digital repository or archival storage entity and
how those packages can be validated.

## Learning Objectives

After completing this lesson, learners should be able to:

* Understand what BagIt is and explain the basic structure of a BagIt digital object.
* Explain why BagIt is useful for digital preservation and what digital preservation and curation functions BagIt may support.
* Identify Python-based and shell tools that can be used to create, analyze, and validate BagIt objects.
* Use the Python `bagit` module to create a BagIt object and generate basic preservation information about a group of files, including fixity information (checksums), inventories (manifests), and other metadata useful for transfer and storage of digital objects.

A longer lesson would include:

* Identify particular use cases and digital curation activities or problems in which BagIt may be a useful tool.
* Significance of validation and how to implement validation using `bagit`.
* How to add contents to a complete BagIt object, update tag metadata, and update manifests. 

## Assumptions

I’m making a few assumptions about what sorts of background you might already have, 
including that you have some level of comfort with the following:

* working with files on a computer (Windows, Mac, Linux, or other filesystem environments),
* that you can find and open files from an Explorer (Windows) or Finder (Mac) graphical interface,
* that you have done a some basic navigation in a shell environment (e.g., Terminal or Bash shell or GitBash) including finding files and directories,
* you have a familiarity with the Python programming language, including using it from an interactive notebook environment (Jupyter notebooks), and
* downloading files from GitHub, opening them on your computer or workstation, and running Jupyter notebooks.

## Learning Resources

1. [Slides for Bagit explanation](BagitOverview.pdf)
1. [Notebook for creating a BagIt object](01b-using-bagit-toteach.ipynb)
1. [Example of a production BagIt object at the National Digital Newspaper Program](https://chroniclingamerica.loc.gov/data/batches/az_acacia_ver01/)

## Notes

This note from [LoC](https://github.com/LibraryOfCongress/bagit-conformance-suite):

* Git's `core.autocrlf` setting can cause bag validation failures by converting CRLF files automatically depending on your operating system and configuration. It is recommended that you disable it in your local checkout of this repository:

  `git config core.autocrlf false`

* Additionally, the below option to run the demonstration in binder may encounter problems since the binder environment may be challenged in running some commands against the virtual file system.
