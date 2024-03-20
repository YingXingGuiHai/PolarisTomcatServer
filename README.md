- [Overview](#overview)
- [Getting Started](#getting-started)
- [Release Notes](#release-notes)

# Overview
[Polaris Tomcat Server](https://plugins.jetbrains.com/plugin/22429-polaris-tomcat-server) is a plugin for Intellij IDEA Community, Ultimate and Educational.  

Highlights:
- One-click to download tomcat
- Auto-detect maven web projects
- Auto-detect gradle web projects
- Auto build artifacts before launch tomcat
- Support launch multiple artifacts
- Support external war files and exploded war directories

The Polaris Tomcat Server supports Tomcat 7 and above.

# Getting Started
### 1. Install PolarisTomcatServer
Search and install PolarisTomcatServer in Intellij IDEA plugin marketplace.
![img](./images/00-PolarisTomcatServer-install.png)

### 2. Download or add tomcat server
Go to Settings -> Polaris Tomcat Server -> Tomcat Servers  -> click Download button to download tomcat server or Add button to add tomcat servers from local disk
![img](./images/01-PolarisTomcatServer-add-tomcat.png)
![img](./images/01-PolarisTomcatServer-download-tomcat.png)

### 3. Add a PolarisTomcatServer configuration
Go to Edit Configuration -> Add New Configuration -> Click Polaris Tomcat Server to add a PolarisTomcatServer configuration
![img](./images/02-PolarisTomcatServer-add-configuration.png)

### 4. Configure tomcat settings
Configure tomcat settings in `Configuration` tab.
![img](./images/03-PolarisTomcatServer-configuration.png)

### 5. Select war artifacts
Go to `Deployment` tab, add war artifacts from web projects or war file.
![img](./images/04-PolarisTomcatServer-deployment.png)
![img](./images/05-PolarisTomcatServer-select-artifacts.png)

# Release Notes
## [1.0.6] - 2024-03-19
- **[Feature]** Support configuration of tomcat admin port, AKA shutdown port.
- **[Improvement]** Remove usage of some deprecated APIs

## [1.0.5] - 2023-12-18
- **[Feature]** Support 'warSourceDirectory' and 'webXml' configuration from maven-war-plugin.
- **[Feature]** Support 'webAppDirectory' and 'webXml' configuration from gradle war plugin.
- **[Feature]** Support plugin recommendation for web projects.
- **[Feature]** Now, the 'Use IntelliJ IDEA API to build artifacts' setting can take effect immediately once configuration panel reopened.
- **[Fix]** An issue that unexpected behaviour when configuration copied.
- **[Fix]** An issue that configuration panel state not changed even if configuration is changed.
- **[Fix]** An issue that artifacts may not be found when configuration is shared across computers.
- **[Fix]** Some display issues.

## [1.0.4] - 2023-12-02
- **[Feature]** Support run tomcat from context (right click menu and main class/method gutter) for web app modules.
- **[Feature]** Support web facet and artifacts
- **[Feature]** Support build artifacts with Intellij APIs.
- **[Feature]** Support filter conditions in download tomcat dialog.
- **[Feature]** Support multiline modifications for artifacts deployment table.
- **[Fix]** Apply button remains enabled after being pressed.
- **[Fix]** Configuration modifications will also modify the configuration template.
- **[Fix]** Some display issues.

## [1.0.1] - 2023-08-14
- **[Fix]** webapp on root context path could not update properly for tomcat 7.x.
- **[Fix]** bugs on windows platform.
- **[Fix]** issue that browser url not changes after port changed.

## [1.0.0] - 2023-08-13
- **[Feature]** One-click to download tomcat
- **[Feature]** Auto-detect maven web projects 
- **[Feature]** Auto-detect gradle web projects 
- **[Feature]** Auto build artifacts before launch 
- **[Feature]** Support launch multiple artifacts 
- **[Feature]** Support external war files and exploded war directories
