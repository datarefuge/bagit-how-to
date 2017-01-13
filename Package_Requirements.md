### Proposed DataRefuge Archival Package Requirements (Shared v1.0) 

Lance Stuchell, University of Michigan Library

Last updated: 1/10/2017

Some assumptions/challenges:

- Because of the urgent nature of this project, data will be archived before full cataloging or other descriptive metadata can be created 
- Files captured through the archiving process may be handed off to other institutions or storage locations, and may be provided to researchers before fully functional access systems are developed
- The information has to be archived in a way that conveys trust in its integrity and authenticity
- Data may be archived by people with differing technical and library skills
- Underlying data format and structure will vary greatly 

To address these challenges, we must: (1) archive data using a minimal level of description, (2) ensure data are transportable to different institutions, storage solutions and users, and (3) document provenance in a transparent manner. In addition, we must employ archiving tools that can be used by people with a range of skill levels. 

**Archival Package Creation**: An archival package will contain, whenever possible, the information necessary to make sense of the data. In some cases this may just be a .warc.gz file, but in other cases it will be a variety of formats and files. This is especially true in cases where automatic web archiving tools cannot be used because of how the data are made available. 

After files are downloaded or created on a local machine (captured), the archival package should be created using the [BagIt packaging format](https://github.com/LibraryOfCongress/bagit-java) as soon as possible. When BagIt packages are made, metadata is automatically generated like the time of package creation, a file manifest, and checksums. Checksums are particularly important, as bit-level integrity can be confirmed in storage or as packages move across institutions and infrastructures. BagIt’s corresponding desktop application, [Bagger](https://github.com/LibraryOfCongress/bagger), can use customized metadata through JSON profiles. 

**Provenance Metadata:** It is unavoidable that content captured from the open internet and stored on local systems will lose some contextual information. It is important that a minimal set of metadata is created at the time of capture to show, as best we can, where this information originated, important characteristics of the data, and who has taken responsibility for its continued preservation. Metadata creation must strike a balance between successfully capturing important information while not overwhelming the package creator. Using a custom profile (profile forthcoming), archiving partners should document:

- UUID (required) 

- - Eg. 68ad27fc-9062-431d-912d-044f6ef2fc4f

- Institution facilitating the data capture creation and packaging (required)

- - Eg: University of Michigan Library 

- Date of capture (required)

- Federal agency data acquired from (required)

- - Eg. Department of Health and Human Services 

- Name of resource (required) 

- - Eg.  GOES Evapotranspiration and Drought (GET-D)

- Individual source or seed URL(s) (required)

- - Eg. [http://www.ospo.noaa.gov/Products/land/getd/index.html](http://www.ospo.noaa.gov/Products/land/getd/index.html), [http://www.ospo.noaa.gov/Products/land/getd/getd-archive-2week.html](http://www.ospo.noaa.gov/Products/land/getd/getd-archive-2week.html), …

- File formats contained in package (required)

- - Eg. warc.gz, .pdf 

- Types of content in package (required)

- - Eg. datasets, reports, codebook

- Free text description of capture process (required)

- - Eg. Metadata for reports were captured through web crawl, individual reports were manually downloaded through the search interface.

- Name of package creator (optional) 

- - Eg. Lance Stuchell 

Metadata will be captured using BagIt’s built-in capabilities and a customized JSON metadata profile (profile is forthcoming). 