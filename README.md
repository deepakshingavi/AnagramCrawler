# AnagramCrawler
Searches a anagram in a huge data set









<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the Project](#about-the-project)
  * [Built With](#built-with)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)



<!-- ABOUT THE PROJECT -->
## About The Project

Application to search for anagrams for given string.


### Built With

* [Maven](https://maven.apache.org/)


<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running follow these simple steps.

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* mvn
* Java 8+

### Installation
 
i. Build the Jar
```sh
mvn clean install
```
ii. Run the Jar (with default Main class)
```sh
java -jar target/AnagramCrawler-1.0.0.jar
```

iii. Run the Jar (with default FileCrawler class to load huge data set from test file)
```sh
java -cp target/AnagramCrawler-1.0.0.jar com.ds.training.main.FileCrawler {file path} {LINE_SEPARATED/SPACE_SEPARATED}
```

Helper Shell scripts
i. build.sh - Run it from project base folder to package the jar
```sh
./shell/build.sh
```
ii. buildAndRun.sh - build and start the default program
```sh
./shell/buildAndRun.sh
```
iii. buildAndRun.sh - build and start main class to upload data from file. 
```sh
./shell/buildAndRunBigCrawler.sh {file path} {LINE_SEPARATED/SPACE_SEPARATED}
```

### Assumptions
i. If the String length in sample data is n then it can vary from 1 < n < 15


### Edge cases
i. Should give memory issue when you start loading files with size > 300 MB on 16GB machine
ii. Ths system cannot be scaled on multiple systems nor utilizes multi threading. 

