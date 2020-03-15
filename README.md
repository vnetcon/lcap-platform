# Low-Code Appliction Platform (LCAP)

For us Low-Code Application Platform (LCAP) is a server and set of tools for fast, easy and cheap:
* REST API development for Web and Mobile Apps
  * Low-Code? Only SQL skills required.
* Data processing for reporting tools
  * Low-Code? Only SQL skills required. 
* Easy way to handle Special Cases (These usually always exist)
  * Talend ESB for Low-Code data processing (Drag and drop visual compnents).
  * Small pieces of java code embedded into Talend if needed (the last option)
* Very easy way to start without installing software
  * Download zip and extract it
  * Start servers with one click
  * Write SQL 
  
In corner cases design your visual no-code Talend job (embed java if needed, hopefully not)  
And on top this we want this to be possible on your own servers __without vendor lock__.  
In short: You can host your servers where ever you want. 

## What is Low-Code Architecture Platform?

This is our extension for LCAP. In all solutions application is always a small part of bigger picture (architecture). Our Low-Code Architecture is a pre-defined architecutre where we have try to reduce the need for coding to minimal. In other words: Authentication etc. are done with ready tools – only some configuration is required. 

Our Low-Code Architecutre Platform is build on following tools:
* __Karaf + vNetCon jdbc-restservlet:__ This is for creating REST APIs with SQL. No need for middle tier coding (e.g. Spring boot rest, php rest etc.).
* __Apache Drill:__ This is for joining multiple data sources (e.g. Oracle, SQL Server, Postgresql) into one with SQL.
* __Karaf + Talend ESB:__ This is an execution environment for rest applications (e.g. jdbc-restservlet) and Talend Jobs (e.g. custom rest services, ETL jobs etc.)
* __Apache http server:__ This is for serving web applicatons (angular, vue, react etc.) and for authentication (e.g. modauth_openidc for OpenID based authentication).

In the next picture you can see the relations between these components as a ”Big Picture architecture view”.


  
![lcap-platform](http://vnetcon.s3-website-eu-west-1.amazonaws.com/img/lcap-architecture.png)


## Easy way to start?
We have try to make this as easy as possible (currently only for Windows 10 64 bit environment). 

1. Download the zip from (comming soon)
2. Extract it into c:\opt
3. Start servers and sql tool (DBeaver) 
3. __Web Devlopment:__ Create REST API with SQL and build your web app against it.
5. __Report development:__ Configure your reporting tool connection to Drill and start report creation. (Before this you need to configure database connections (Oracle, SQL Serveer etc.) to drill).

More detailed instructions can be found in wiki pages.  
Below is a picture of the folder structure after extracting the zip.  
![lcap-platform-unzipped](http://vnetcon.s3-website-eu-west-1.amazonaws.com/img/unzipped.png)

  
 ## What does the zip include?
* __Openjdk 1.8:__ This is needed for Drill, Karaf etc.
* __Apache http server:__ This is for serving web applications.
* __Apache Drill:__ This is for joining external datasources to one with SQL.
* __Apache Karaf:__ This is a Talend ESB version of karaf + vNetCon web apps (e.g. jdbc-restservlet for SQL based REST API creation). 
* __DBeaver:__ The open source version of DBeaver for executing SQL statements against different databases.
* __Talend TOS for ESB:__ This is Talend Studio for creating Talend Jobs by drag and dropping components and connect those with ”arrows”.
  
In short all you need to develop REST API:s for your web applications and prepare data to your reporting tool.

## What does this cost?
If you want to keep your code closed 99 USD. 
  
vNetCon’s Open Source code is licensed under AGPL-3.0 and we sell 99 USD licenses for closed code projects and applications.
You can buy the license online at https://vnetcon.com
  
If you think the price is too high/low you can change the price to level you think is correct.


