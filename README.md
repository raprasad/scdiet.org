# scdiet.org

Archive of the original SCDiet.org site created by [Mik Aidt](https://twitter.com/mikaidt) and [Mike Simons](http://www.glassbird.com/)

Created to help people using Elaine Gottschall's version of the Specific Carbohydrate Diet (SCD), from 1996 through September 2016, this site lived at ```www.scdiet.org```.

As described in the site's footer:

```
The SCD Web Library contains approximately 8.1 megabytes of listserve archives and information about the SCD, app. 350 webpages equal to approximately 3,800 typed
A4 papersheets.
```

This archive contains the static HTML and images from the site.

Please see the versions tab for:

  1. The original version where pages were hardcoded with links to "http://www.scdiet.org"
  1. The "archive subdirectory" where the files may be placed in the subfolder of an existing web server.
    - For this version, do a search/replace over all of the files, changing:
      - **From**: ```||ARCHIVE_SUBDIRECTORY||```
      - **To**: your folder name.  e.g. ```archive``` (don't include slashes)

Example of running the "archive subdirectory" version

  - Replace ```||ARCHIVE_SUBDIRECTORY||``` with ```scdarchive```
  - Save the files.
  - In the repository folder, run a python server
```
cd scdarchive
python -m SimpleHTTPServer 8000
```

- Go to http://0.0.0.0:8000/scdarchive


---

## Replace sequences

### Original version to "archive subdirectory" version

Here is the replace sequence run to go from the original version to one which may be served from the subdirectory of a webserver.

 - REPLACE ```href="http://www.scdiet.org/``` WITH ```href="/||ARCHIVE_SUBDIRECTORY||/```
 - REPLACE ```href="http://www.scdiet.org"``` WITH ```href="/||ARCHIVE_SUBDIRECTORY||"```
 - REPLACE ```src="http://www.scdiet.org/``` WITH ```src="/||ARCHIVE_SUBDIRECTORY||/```
 - REPLACE ```value="http://www.scdiet.org/``` WITH ```value="/||ARCHIVE_SUBDIRECTORY||/```
 - REPLACE ```xml:base="http://www.scdiet.org/news``` WITH ```xml:base="/||ARCHIVE_SUBDIRECTORY||/news```
 - REPLACE ```URL=http://www.scdiet.org"``` WITH ```URL=/||ARCHIVE_SUBDIRECTORY||"```
 - REPLACE ```HREF="http://www.scdiet.orgdk``` WITH ```href="/||ARCHIVE_SUBDIRECTORY||/dk```
 - REPLACE ```open ("http://www.scdiet.org/``` WITH ```open ("/||ARCHIVE_SUBDIRECTORY||/```
