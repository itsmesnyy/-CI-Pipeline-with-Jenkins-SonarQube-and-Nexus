CI/CD PIPELINE WITH JENKINS, SONARQUBE, AND NEXUS
=================================================

PROJECT OVERVIEW
----------------
This project demonstrates a complete CI/CD pipeline using Jenkins, SonarQube, and Nexus Repository. 
The pipeline automates the following steps:

1. Code checkout from GitHub
2. Tool installation and build
3. Unit testing
4. Static code analysis with Checkstyle and SonarQube
5. Enforcing a SonarQube quality gate
6. Uploading the artifact to Nexus repository (only if quality gate passes)

DESCRIPTION
-----------
This project demonstrates a robust CI/CD pipeline designed using Jenkins to automate the software development lifecycle of a Java-based application. It integrates essential DevOps tools like GitHub, Maven, SonarQube, and Nexus to ensure reliable and quality-driven deployments.

The pipeline performs a sequence of steps starting with fetching the source code from a GitHub repository. It then compiles and builds the application using Maven, runs unit tests, and performs static code analysis with SonarQube and Checkstyle. The pipeline enforces a quality gate — if the code passes the analysis criteria, the final artifact is uploaded to a Nexus repository for versioned storage and future deployment.

This setup enforces DevOps best practices such as continuous integration, early detection of bugs, code quality enforcement, and artifact versioning. It is highly scalable and can be adapted to support containerized deployments, cloud environments, and microservices architectures.


TOOLS & TECHNOLOGIES USED
-------------------------
- Jenkins                  : CI/CD pipeline automation
- GitHub                   : Source code management
- Maven                    : Project build and dependency management
- Checkstyle               : Code style analysis
- SonarQube                : Static code analysis
- Nexus Repository Manager : Artifact storage

PIPELINE STAGES
---------------
1. Checkout SCM          : Clones the GitHub repository.
2. Tool Install          : Installs required tools (e.g., Maven, Java).
3. Build                 : Compiles the code using `mvn clean install`.
4. Test                  : Runs unit tests.
5. Checkstyle Analysis   : Validates code style using Checkstyle.
6. Sonar Analysis        : Sends analysis to SonarQube.
7. Quality Gate          : Waits for SonarQube's approval.
8. Upload Artifact       : Uploads the build artifact to Nexus if the quality gate is passed.




SCREENSHOT
----------


