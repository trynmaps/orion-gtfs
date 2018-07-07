# orion-gtfs
Gets GTFS sources from config and uploads them to S3

AWS Lambda Function runs hourly and updates the GTFS source files with the ones linked to in the config.

## Purpose

We need a single reliable. source for GTFS files for each agency. Uploading them to S3 gives us versioning in case a GTFS update is broken (or just happens to break us) along with durability in case the agency changes the path of its GTFS or if it disappears.

## Usage

This GTFS is used by all our services and clients
