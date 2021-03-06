# Number to Words
Converts numbers to their English word equivalents. The supported range is -2,147,483,648 to 2,147,483,647.

## What you'll need
1. Maven 3.6.0+.
1. JDK 8 or later.
1. Latest version of Docker (if you plan to build and run through Docker).

## Building the jar
1. Run `mvn package` to build the jar file. This will also run the tests.

## Running the jar
1. Run `java -jar <name of jar file> <list of numbers delimited by spaces>`.
    - eg: `java -jar interview-1.0-SNAPSHOT.jar 43242 678`.

## Docker build
1. Run `docker build -t <image namespace>/<image tag> .`
    - eg: `docker build -t exercise/numbers-to-words .`

## Running the Docker container
1. Run `docker run <name of image from build step> <list of numbers delimited by spaces>`
    - eg: `docker run exercise/numbers-to-words 43242 678`
1. Alternatively you can use what's already on Docker Hub.
    - eg: `docker run gantderising/numbers-to-words 43242 678`
