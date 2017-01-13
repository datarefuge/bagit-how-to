# bagit-how-to


## Principles:

- If a site can be included in the Internet Archive, it should be.
- This data catalog to for preserving and providing access to federal environmental and climate datasets that can not be captured as warc files.
- When in doubt about where to put tricky sites/datasets, go for both warc in IA and here as bagit files.

**Note for tech people**

You will need to work with two technologies for this project that you might not be familiar with. They are both standards for preserving digital files that are widely used for preservation and continued access. There are lots of resources for learning more about them. In the meantime, the basics:

**WARC files** - (see picture!) If you've ever seen the Wayback machine on the Internet Archive, it's made up of WARC files. This is basically a wrapper used to store and serve archived copies of websites.

**BAGit Bags** - [Bagit](https://en.wikipedia.org/wiki/BagIt) is a standard for storing arbitrary sets of files in ways that ensure their continuity as they move around. Why use them in this case? Because, if we're dealing with files that can't be nicely re-created using warc files, they will need to be described and catalogued to make them easy to find. This will take time. In the meantime, we want to ensure their existence and make sure they are citable and available. The bagit standard is widely used for digital preservation. See package requirements for more info.
