NPM SFDX Package Dependancy Resolution Proof of Concept
1. Open git bash on windows with npm... and sfdx... and a default devhub org*
2. Clone repo

  ```bash
  git clone [URL]
  ```

3. cd into repo

  ```bash
  cd fflib-apex-common-samplecode
  ```

4. Install the QRFDev Package Manager tools

  ```bash
  npm install qfpm --save --only=prod
  ```

5. Setup for development

  ```bash
  npm run setup
  ```

6. Oh no this package has multi-layered dependancies needed to install!
  
7. Install the npm-fflib-common dependancy

  ```bash
  npm install npm-fflib-common --save --only=prod
  ```

8. Setup again with dependacies installed

  ```bash
  npm run setup
  ```

9. You now have a scratch org ready for development with multiple layers of dependancies resolved

*May work on linux though has not been tested

Original README Below
=====================

FinancialForce Apex Common Sample
=================================
=======
FFLib Apex Common Sample
========================

**Dependencies:** Must deploy [Apex Mocks](https://github.com/apex-enterprise-patterns/fflib-apex-mocks) and [Apex Common](https://github.com/apex-enterprise-patterns/fflib-apex-common) before deploying this library

Deploy Apex Mocks
<a href="https://githubsfdeploy.herokuapp.com?owner=apex-enterprise-patterns&repo=fflib-apex-mocks">
  <img alt="Deploy to Salesforce"
       src="https://raw.githubusercontent.com/afawcett/githubsfdeploy/master/src/main/webapp/resources/img/deploy.png">
</a>

Deploy Apex Common
<a href="https://githubsfdeploy.herokuapp.com?owner=apex-enterprise-patterns&repo=fflib-apex-common">
  <img alt="Deploy to Salesforce"
       src="https://raw.githubusercontent.com/afawcett/githubsfdeploy/master/src/main/webapp/resources/img/deploy.png">
</a>

Deploy Apex Common Sample Code
<a href="https://githubsfdeploy.herokuapp.com?owner=apex-enterprise-patterns&repo=fflib-apex-common-samplecode">
  <img alt="Deploy to Salesforce"
       src="https://raw.githubusercontent.com/afawcett/githubsfdeploy/master/src/main/webapp/resources/img/deploy.png">
</a>

Sample Application
==================

This repository contains a sample application illustrating the Apex Enterprise Patterns library. The aim is to illustrate fullly working sample application to better illustrate the patterns in presentations and articles. You can see a [demo of this application in the Dreamforce 2013 session](http://www.youtube.com/watch?v=qlq46AEAlLI#t=572) presented by @afawcett

**NOTE:** The supporting **Apex Common** library can be found [here](https://github.com/apex-enterprise-patterns/fflib-apex-common).

![Alt text](/images/sampleappoverview.png "Optional title")

Application Enterprise Patterns on Salesforce Lightning Platform
================================================================

Design patterns are an invaluable tool for developers and architects looking to build enterprise solutions. Here are presented some tried and tested enterprise application engineering patterns that have been used in other platforms and languages. We will discuss and illustrate how patterns such as Data Mapper, Service Layer, Unit of Work and of course Model View Controller can be applied to Force.com. Applying these patterns can help manage governed resources (such as DML) better, encourage better separation-of-concerns in your logic and enforce Force.com coding best practices.

Dreamforce Session and Slides
-----------------------------

- View slides for the **Dreamforce 2013** session [here](https://docs.google.com/file/d/0B6brfGow3cD8RVVYc1dCX2s0S1E/edit) 
- Video recording of the **Dreamforce 2014** advanced session [here](https://www.youtube.com/watch?v=BLXp0ZP0cF0).
- View slides for the **Dreamforce 2015** session [here](http://www.slideshare.net/andyinthecloud/building-strong-foundations-apex-enterprise-patterns)

More Information on Trailhead
--------------------------------------------

There are two Trailhead Modules for Apex Enterprise Patterns:

- [Apex Enterprise Patterns - Service Layer](https://trailhead.salesforce.com/en/content/learn/modules/apex_patterns_sl)
    - [Separation of Concerns](https://trailhead.salesforce.com/en/content/learn/modules/apex_patterns_sl/apex_patterns_sl_soc)
- [Apex Enterprise Patterns - Domain and Selector Layer](https://trailhead.salesforce.com/en/content/learn/modules/apex_patterns_dsl)

