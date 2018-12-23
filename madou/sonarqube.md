


## SonarQube
The SonarQube Platform is made of 4 components:
![](../images/madou/img-000.jpg)

1. One SonarQube Server starting 3 main processes:
    - Web Server for developers, managers to browse quality snapshots and configure the SonarQube instance
    - Search Server based on Elasticsearch to back searches from the UI
    - Compute Engine Server in charge of processing code analysis reports and saving them in the SonarQube Database
2. One SonarQube Database to store:
    - The configuration of the SonarQube instance (security, plugins settings, etc.)
    - The quality snapshots of projects, views, etc.
3. Multiple SonarQube Plugins installed on the server, possibly including language, SCM, integration, authentication, and governance plugins
4. One or more SonarScanners running on your Build / Continuous Integration Servers to analyze projects


We can work online on SonarQube in the last versions but we will be installing it locally for this project, let’s start with installing and lunching SonarQube:  

![](../images/madou/img-001.jpg)


After unzipping the content of the zip downloaded in `C:\SonarQube-7.4` foe example, we can start it with a simple command 
`C:\SonarQube-7.4\bin\windows-x86-64\StartSonar.bat`
Then going to http://localhost:9000 we will see the home page of SonarQube 

![](../images/madou/img-003.jpg)


To test SonarQube we will be using maven project, so we need to add sonar plugin into `pom.xml`

![](../images/madou/img-004.jpg)


After running clean and install, we can run `sonar:sonar` plugin

![](../images/madou/img-005.jpg)


After a build success we can now open http://localhost:9000 to observe this interface that contains the projects analyzed by SonarQube and the detected issues.

![](../images/madou/img-006.jpg)


Thus in intelIj we can add a plugin called SonarLint that do scan the code for issues and errors

![](../images/madou/img-007.jpg)
