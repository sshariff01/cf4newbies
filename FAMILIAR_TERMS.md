# Familiar Terms


### Buildpacks

* Buildpacks allow CF to support multiple languages and deployment environments.


### Manifests

* A manifest is a deployment "blueprint" for an application. In other words, a specification of how your application runs.



### Organizations

Cloud Foundry is designed for use by organizations supporting collaboration. An organization defines one or more domains. A Cloud Foundry instance defines a default domain for all organizations. You may also add your own subdomains. 


### Spaces

* Organizations contain one or more spaces
* Within PWS, the default spaces are `development`, `test`, and `production`
* Users can create additional spaces
* Many applications can run and scale within a space


### Users and Roles

* Members of an organization
* Your role defines your permissions to access and modify applications

#### Organization Roles

**Organization Manager** - Can invite/manage users, select/change the plan, establish spending limits, etc.

**Organization Auditor** - View-only access to all organization and space info, settings, and reports

#### Space Roles

**Space Manager** - Can invite/manage users, enable features for a given space

**Space Developer** - Can create, delete, manage applications and services, full access to all usage reports and logs

**Space Auditor** - View-only access to all space information, settings, reports, logs

### Domains

* Every deployed application is associated with a unique URL
* All requests to that URL redirect to the application
* Each CF instance has a default domain
* You can register your own domain and give it to Cloud Foundry to use and manage
* Every application has a unique sub-domain of the master domain

### Routes

* While domains can be mapped to multiple spaces, a route can only be mapped to **one** space

### Services

* Anything that you need to provision alongside your application is a service (i.e. database, messaging service, etc.)
* Services are usually bound to one or more applications
* **Note:** All configuration data to CF applications are passed through environment variables (not configuration files, since there is no filesystem)