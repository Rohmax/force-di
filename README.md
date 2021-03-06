# Force DI

Generic [DI](https://en.wikipedia.org/wiki/Dependency_injection) library with support for injecting Apex, Visualforce and Lightning code at runtime. 

Documentaiton
-------------
- [General overview of the library features, configuration and use of Injectors](https://andyinthecloud.com/2018/07/15/managing-dependency-injection-within-salesforce/)
- [Using the library to aid with Test Driven Development in Apex](https://andyinthecloud.com/2018/07/29/test-driven-development-mocking-and-force-di/)
- [Dependency Injection, Flows, and Force DI](https://douglascayers.com/2018/08/05/dependency-injection-flows-and-force-di/)
- [Adopting Dependency Injection](https://douglascayers.com/2018/08/29/adopting-dependency-injection/)

Project Folders
---------------

![Force DI Example](https://andrewfawcett.files.wordpress.com/2018/07/forcedi2.png)

| Folder | Description |
| ------ | ----------- |
| **force-di** | Core library, contains **Injector** Apex API and **<c:di_injector>** VF and Lightning Components |
| **force-app-1** | Sample application using the API and Components to inject Apex, VF and Lightning at runtime |
| **force-app-2** | Sample package providing impls for various bindings above |
| **force-app-3** | Sample package providing impls for various bindings above |
| **force-di-trigger-demo** | Sample basic trigger framework leveraging the API |

Install latest version via a Salesforce DX Package
--------------------------------------------------

You have two options you can install via your web browser [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t1N000000Cr7oQAC) or you can install via the Salesforce DX CLI as shown below.

~~~~
sfdx plugins:install shane-sfdx-plugins
sfdx shane:github:package:install -g afawcett -r force-di
~~~~

Other Resources on Dependency Injection Design Pattern
------------------------------------------------------

Some of these blogs and videos are not necessarily Salesforce-specific but give good insights on use cases and purpose behind this design pattern.

### Videos

- [Dependency Injection Overview](https://www.youtube.com/watch?v=IKD2-MAkXyQ&t=0s&index=3&list=PL-oxrNbxQl3-wPOf0t3PT-0JYXiOBwReG) by Anthony Ferrara
- [Advanced Apex Design Patterns](https://www.youtube.com/watch?v=IKD2-MAkXyQ) by Andy Fawcett
- [Writing True Unit Tests Using Dependency Injection and Mocking](https://www.youtube.com/watch?v=hj4538vR6Mg&list=PL-oxrNbxQl3-wPOf0t3PT-0JYXiOBwReG&index=4) by Alex Tennant

### Blogs

- [Injection Design Pattern](https://martinfowler.com/articles/injection.html) by Martin Fowler
- [Dependency Injection is not the same as Dependency Inversion](https://lostechies.com/derickbailey/2011/09/22/dependency-injection-is-not-the-same-as-the-dependency-inversion-principle/) by Derick Bailey
- [Dependency Injection](https://stackify.com/dependency-injection) by Thorben Janssen
