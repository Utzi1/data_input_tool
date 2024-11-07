# Concept

To enable a seamless data input to the redis database used for the SURGEAHEAD,this module will be constructed.
As later all parts will be run in Containers (Docker, Packman, etc.), this circumstance will be part of the design.
Here a few points to consider:

* A Flutter web app can't directly connect to a Redis database.
* The Flutter web app can connect to a REST API.
* Communication between the Flutter web app and the REST API is done via HTTP.
* The REST API can connect to a Redis database.
* Overall a strict handling of the input data is necessary to avoid data corruption.
