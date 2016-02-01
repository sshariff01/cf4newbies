# Using the Cloud Foundry CLI


## The .cf Direcory

cf creates a `.cf` directory in your home directory, where it stores context, logs, crash reports, etc., along with remembering your CF API endpoint.


## Deploy Using the CLI

To deploy an application, you need an application that is ready to be deployed. For some applications, depending on the nature of the technology they have been developeed with, the application may need to be built first. For example, a Java application may need to be built with build tool to produce a .jar or .war. Other languages, such as Ruby or Node.js, are interpreted don't need to built. 

Once you have a deployable application, it can be deployed using `cf push <app-name>`. Run `cf help push` in your Mac OS X terminal for additional usage details.


## Domains and URLs

Every CF instance is assigned a domain at installation. For Pivotal Web Services, this domain is `cfapps.io`. When you deploy, your application gets a URL to access it. For example, when deploying an application with `cf push <app-name>`, the generated URL looks like `<app-name>.cfapps.io`.


## Configuring a Deployed Application

### Change the number of instances

* `cf scale <app-name> -i <new-value-number-of-instances>`

### Change the memory allocation

* `cf scale <app-name> -m <new-value-memory-allocation>`

### Change domain mappings

* `cf map-route <app-name> <domain> -n <route>`
* `cf unmap-route <app-name> <domain> -n <route>`


## Useful Commands

* `cf apps` - List of apps running in your organization 

* `cf app <app-name>` - View the configuration of an application

* `cf logs <app-name>` - Get tailed logs of an application

* `cf stop <app-name>` - Stop all application instances

* `cf start <app-name>` - Start all application instances



