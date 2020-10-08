# Rasa Advanced Workshop: Externalizing Responses

Responses server written in Java that exposes a REST API adhering to Rasa [responses](https://legacy-docs.rasa.com/docs/core/responses/) format.
The advantage of this is small bot utternaces can be easily modifed without retraining the model, thereby
improving the development time.

## Development
This project is developed on top of [vert.x](http://vertx.io/) using JDK 11.

* Install the latest version of JDK 11.
docker run -it --rm -v "$PWD":/workshop -v "$PWD/.m2":/root/.m2/ -w /workshop -p 8080:8080 openjdk:11 bash
* Build the code by running the maven wrapper "./mvnw clean install"
* To start the server, run "java -jar target/workshop-1.0.0-SNAPSHOT-fat.jar"

## Credits
Repurposed from https://github.com/floc-crisis-center
