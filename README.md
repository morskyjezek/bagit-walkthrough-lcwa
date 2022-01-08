# Demonstrating BagIt Concept and Tools

This repository holds materials for use in learning digital curation tools and concepts from archival and library perspectives. Specifically, this repository explains the **BagIt** concept and associated, Python-based tools; these concepts and tools are demonstrated using sample files from the Library of Congress Web Archvies (LCWA). This short demonstration lesson was created as part of work on a larger set of lessons that outlines additional digital curation and preservation actions associated with all elements of the digital curation lifecycle.

## Lesson Concept: Demonstrate BagIt Structure and Creation Tools

Using the BagIt standard, this repository outlines the elements
of file packages created according to the BagIt structure ("bags"),
how to organize files for these structures, initiate them with Python-based
tools, and how to analyze, update, and plan them.

The use case here is to explain how to create file packages that can be
reliably transmitted to a digital repository or archival storage entity,
how those packages can be validated, and how this structure is used
in various repositories managed by institutions.

The demonstrates shows how you can use BagIt and associated tools to
generate basic preservation information about a group of files,
including create of fixity information (checksums),
inventories (manifests), and other metadata useful for transfer and storage of digital objects.

## Notes

This note from [LoC](https://github.com/LibraryOfCongress/bagit-conformance-suite):

* Git's `core.autocrlf` setting can cause bag validation failures by converting CRLF files automatically depending on your operating system and configuration. It is recommended that you disable it in your local checkout of this repository:

  `git config core.autocrlf false`

* Additionally, the below option to run the demonstration in binder may encounter problems since the binder environment may be challenged in running some commands against the virtual file system.

## Try it in Binder

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/morskyjezek/bagit-walkthrough-lcwa/main)
