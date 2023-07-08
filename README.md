# SonarQube Scanner for Gradle

<p align="center">
<a href = "https://medium.com/@sagarkrp/how-to-install-and-configure-sonarqube-with-jenkins-2fe6c732620" target ="_blank">
<img alt="NGINX" width="270px" src="https://raw.githubusercontent.com/devicons/devicon/develop/icons/sonarqube/sonarqube-original-wordmark.svg" style="padding-right:10px;" />  </a>
</p>
</br>
<h3> <strong> Read the detailed article on: </strong> </h3> <a href = "https://medium.com/@sagarkrp/how-to-install-and-configure-sonarqube-with-jenkins-2fe6c732620" target ="_blank"> 
 
<picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/sagarkrp/sagarkrp/blob/main/images/Medium-white1x.png" width="180px" height="45px">
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/sagarkrp/sagarkrp/main/images/Medium-dark.svg" width="180px" height="45px"> 
   <img alt="Medium Alternative Theme." src="https://raw.githubusercontent.com/sagarkrp/sagarkrp/main/images/Medium-dark.svg" width="180px" height="45px">
</picture> </a>


This example demonstrates how to analyze a simple project built with [Gradle](https://gradle.org/).

<!-- <p> <strong> Read the detailed article on: </strong> </p> <a href = "https://medium.com/@sagarkrp/how-to-install-and-configure-sonarqube-with-jenkins-2fe6c732620" target ="_blank"><img src = "https://img.shields.io/badge/medium-%23E4405G.svg?&style=for-the-badge&logo=medium&logoColor=black&white"></a> -->

## Prerequisites

* [SonarQube](http://www.sonarqube.org/downloads/) 9.9 LTS or Latest
* A gradle wrapper is included that bundles gradle. All other required plugins will be pulled by gradle as needed.

## Usage

Run the following command (updating the sonar.host.url property as appropriate):

* On Unix-like systems:
  `./gradlew -Dsonar.host.url=http://myhost:9000 sonar`
* On Windows:
  `.\gradlew.bat -D'sonar.host.url=http://myhost:9000' sonar`

## Coverage

To get the project [test coverage](https://community.sonarsource.com/t/coverage-test-data-importing-jacoco-coverage-report-in-xml-format) computed, add gradle task `jacocoTestReport` to your command line.
