# bagit-how-to


## Principles:

- If a site can be included in the Internet Archive, it should be.
- This data catalog to for preserving and providing access to federal environmental and climate datasets that can not be captured as warc files.
- When in doubt about where to put tricky sites/datasets, go for both warc in IA and here as bagit files.

Overview:
You and your team can choose from a set of available sites that can't be crawled by a web crawler. Your task is to get the data from that site as completely as possible, document what you've done, and move the copy of the data into a preservation format. Ask your guide for more info.
Basically, you'll:

1. Identify a website you'd like to work on from the spreadsheet, and claim it.
1. Download data from federal website, and associated files, websites, etc.
1. Use bagit to wrap the files up into a bag.
2. Create a record in CKAN instance at [datarefuge.org](http://www.datarefuge.org) for your bag
   1. Use the Holding Organization (ask your guide for login credentials)
   2. Create appropriate metadata using the form
3. Request an uploader over slack, and raise your card - prepare your bag to be moved to S3 by an Uploader (they have permissions to an AWS S3 bucket that will store the data)
4. Update the spreadsheet to note that this tricky site is done.
5. On to the next!


**Note for tech people**

You will need to work with two technologies for this project that you might not be familiar with. They are both standards for preserving digital files that are widely used for preservation and continued access. There are lots of resources for learning more about them. In the meantime, the basics:

**WARC files** - (see picture!) If you've ever seen the Wayback machine on the Internet Archive, it's made up of WARC files. This is basically a wrapper used to store and serve archived copies of websites.

**BAGit Bags** - [Bagit](https://en.wikipedia.org/wiki/BagIt) is a standard for storing arbitrary sets of files in ways that ensure their continuity as they move around. Why use them in this case? Because, if we're dealing with files that can't be nicely re-created using warc files, they will need to be described and catalogued to make them easy to find. This will take time. In the meantime, we want to ensure their existence and make sure they are citable and available. The bagit standard is widely used for digital preservation. See package requirements for more info. There is also a good overview of bagit and instructions for using it [http://metaarchive.org/public/resources/neh/research/BagIt_Usage_Instructions.pdf](http://metaarchive.org/public/resources/neh/research/BagIt_Usage_Instructions.pdf)
