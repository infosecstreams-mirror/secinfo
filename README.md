# Secinfo [DEPRECATED]

> **⚠️ DEPRECATION NOTICE: This tool is no longer in use by the infosecstreams-mirror project.**
> 
> Historically, this codebase ran as a GitHub Action that read `streamers.csv` and statically generated markdown files for the frontend website. 
> 
> Our new architecture relies entirely on the **[StreamStatus](https://github.com/infosecstreams-mirror/StreamStatus)** Go REST API, which stores real-time streamer statuses in a PostgreSQL database and serves them dynamically to the decoupled frontend.
>
> This repository is kept for historical/archival purposes and upstream syncs only.

## Original Documentation

This is code in Golang that will read a csv file and generate updated markdown files to be displayed on https://github.com/infosecstreams-mirror/infosecstreams-mirror.github.io/

### Development

Check the `Makefile` for all options but you've got `make {docs,test,cover,clean,build,docker-build,docker-run}` available to you.

When running `docker-run`, we assume you're providing `streamers.csv` from the infosecstreams repo. You can check the invocation of the `docker run ...` command in the Makefile for further details.
