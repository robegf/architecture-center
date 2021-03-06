# Artifact Repository

![Nexus](./../resources/images/components/nexussnapshot.png)

The artifact repository delivered by Talend and based on Sonatype Nexus is a preconfigured application centralizing the management and usage of the Software Update, User libraries and snapshots and releases repositories:

- Software Update is used to manage application updates (patches) distributed by Talend. 
- The User libraries repository is used to store all external libraries. 
- The snapshots and releases repositories are used as a catalog in which all artifacts to be deployed and executed are stored. These artifacts are designed by the user from the Studio or any other Java IDE. By default, the snapshots repository is used for development purposes and the releases repository is used for production. These repositories make artifacts available for deployment and or execution in an execution server.

#### Technical Details:
- TAC defines the URL’s to the nexus repository for Studio
- It is a server component and runs as a service.
- It is a web application and is accessed via a web browser
- Generally, it is recommended to have just one instance which is used to deploy to all environments
- One instance of Nexus can manage several repositories. Talend uses five repositories in its default configuration  
- Only Nexus Releases and Snapshots repositories are accessible to TEST and PRE-PROD environments.
- Only Releases repository is accessible from PROD environment.
- Nexus access can be controlled by user privileges and firewall/proxy.
- Installed by the Installer or use your own – Only Sonatype Nexus 2.14 is supported. Nexus 3 will not work
- Critical for Talend development environment to function correctly!

To read in detail about Artifact repository please click [link][Artifact-Repository] 

To read more on Publishing into the Artifact repository please click [link][Publishing-To-Artifact-Repository]

<!-- links -->
[Artifact-Repository]: https://help.talend.com/reader/FA4p9lNzB_hO9dnUE0EnqA/1TFowu9A8_5OWB0AcpJthA "Artifact Repository Details"
[Publishing-To-Artifact-Repository]: https://help.talend.com/reader/nXPtKhielAtSqFD6_f7~OQ/1tHg0_3RUgymE7Gq8c0bmA "Publishing into the Artifact repository"
