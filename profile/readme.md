# 4D Genome Browser toolkit

The 4D Genome browser toolkit is a collection of tools, algorithms and viewers for genomics data, created by Los Alamos National Laboratory.

## 4D Genome Browser

The 4D Genome Browser is a toolkit for querying and visualizing genomics data through the web. It consists of a few different components:

- A web server that responds to queries for data and serves either raw JSON data or webpages displaying visualizations of the data.
- A python library for making requests to such a server
- A Javascript browser library for visualizing data.

Data is formatted into "projects". A project consists of all of the input data files and a project.json file describing the files along with settings for viewing them. A project can then be "compiled", having all of its data incorporated into an SQLite database. This database is what the web server queries to serve data. A "release" of a project consists of a copy of the server code, the projectg directory, the project database, static files (including a minified version of the javascript library) along with a copy of the python library for querying the server.
