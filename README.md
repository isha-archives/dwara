# Dwara

--------------
What is Dwara?
--------------

Dwara is a general purpose framework for the management, storage and processing of digital data, with a focus on enabling the activities needed for digital preservation. 

For the purpose of product comparison, Dwara can be viewed as sitting somewhere between the following types of system:

* Digital Asset Management
* Software Defined Storage
* Process Automation

Dwara is storage and data agnostic, and provides an API for defining new data storage interfaces and custom data processing tasks. Complex automation flows can be created with dependency chaining and static and dynamic configuration options. These can be applied to different sets of data during ingest or at any other point in the data lifecycle. A full record of all task executions is maintained to facilitate comprehensive auditing and analysis at any point in time.

-----------------
Who is Dwara for?
-----------------

Dwara is for any organization that needs to store and process large amounts of data in an automated way. It was designed with the objective of facilitating the activities needed for long term data preservation, (although the framework is not necessarily limited to that use case). 

Dwara is not meant to be used off the shelf - depending on the user requirements there may be a need for custom processing modules to be developed by the user. Furthermore, Dwara has a fairly complex setup and configuration which requires a good technical person to undertake. 

------------------------------
Dwara for Digital Preservation 
------------------------------

Portico defines **digital preservation** as:

   *A series of management policies and activities necessary to ensure the enduring usability, authenticity, discoverability, and accessibility of content over the very long term.*

Digital preservation presents several key challenges, which Dwara can help address:

| Storing large volumes of data inexpensively           | Dwara can be configured to store copies of data on different storage media types. This can be done to reduce the risk of data loss, and also allows data to be transitioned to a lower cost storage type without any disruption.                                                                                |
| Maintaining data integrity and authenticity           | Dwara stores a checksum for every file ingested as well as the date the checksum was last verified, allowing periodic fixity checking of data to be scheduled.                                                                                                                                                  |
| Migrating data to new storage media                   | Flows can be defined to automatically restore artifacts from older storage volumes, verify all file checksums, and rewrite them to one or more new storage volumes, recording the storage history of each artifact.                                                                                             |
| Converting data to preservation friendly file formats | Similarly, flows can be defined to automatically restore artifacts of a certain type, apply custom processing to convert the files to another format, and write the new artifacts to storage, linking the derived artifact to the source artifact.                                                              |
| Maintaining descriptive metadata                      | Dwara can call external applications to extract useful metadata from files being ingested. User defined tags can be added to artifacts, which can be used for searching and filtering files for different types of processing.                                                                                  |
| Providing quick retrieval of data when needed         | Dwara allows users to search for ingested artifacts and restore the files they need, allowing queued restore jobs to be dynamically reprioritized. For media content the framework allows PFR (partial file retrieval) flows to be implemented for different combinations of storage formats and media formats. |
| Handling private data                                 | Private data can be stored on separate physical volumes and also be subject to modified processing flows. For example, inclusion of an additional encryption task, or exclusion of a default publishing task during data ingest.                                                                                |






