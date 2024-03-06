# Instructions to set up Blazegraph for the Open SbD4Nano Semantic Landscape data

This repository contains instructions for using [Blazegraph](https://github.com/blazegraph/database) locally to host a SPARQL
endpoint with the open SbD4Nano Semantic Landscape data. Blazegraph is no longer
actively developed and Virtuoso or [QLever](https://github.com/h2020-sbd4nano/sbd-data-landscape-qlever)
may be more appropriate solutions.

## Creating and starting

First, download the most recent `blazegraph.jar` release from [this page](https://github.com/blazegraph/database/releases).
You need a Java environment, and you can start blazegraph then with:

```shell
java -jar blazegraph.jar
```

This will fire up a webpage and SPARQL endpoint, e.g. at `http://localhost:9999/blazegraph/`.
Go to the Update tab and load the Turtle file of the open data. For large files, using the
'Type' "File Path or URL" is recommended. The URL https://raw.githubusercontent.com/h2020-sbd4nano/sbd-data-landscape-opendata/main/open.ttl
can be used.

## Querying the SPARQL endpoint

In the webinterface you can run SPARQL queries in the "Query" tab. 

From the command line, the URL for the endpoint is: http://localhost:9999/blazegraph/sparql
