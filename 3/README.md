# 3. Configuration Indexer

The Goobi viewer relies on Apache Solr to search metadata and full texts. 

To make new records known to the Goobi viewer, they must first be indexed. This task is performed by the Goobi viewer Indexer. Once started, it monitors a folder in the file system, the so-called hotfolder. It accepts tasks via this folder, for example to re-index records, but also to update or delete existing records. 

The configuration takes place in the file `solr_indexerconfig.xml` in the installation path of the Goobi viewer indexer. This is usually `/opt/digiverso/indexer`. The configuration options are described in more detail in the following subchapters.

