# Introduction to Using Cloud Foundry with Spring Tool Suite


## Prerequisites

### Required

* Setup a Pivotal Web Services trial account
* Install the Cloud Foundry Command Line Interface

### Optional 

#### Installing and Setting Up Spring Tool Suite

1. Install [Spring Tool Suite](http://spring.io/tools/sts)

2. Install Cloud Foundry Integration with STS    
    * Within STS, go to `Help > Install New Software` and search for "Cloud Foundry". Install these required packages. Note that the install process may take a bit of time, and STS will need to be restarted for the changes to take effect.
    
3. Import projects into STS
    * Install samples and partially-completed projects into your workspace. Run the following command in your Mac OS X Terminal:
    ```
	git clone https://github.com/s2edu/cloudfoundrystudentfiles
    ```
    
    * From the project explorer, right click: `Import > Maven > Existing Maven Projects`
	
    * Navigate to the folder where you extracted the student files (step 3a) and Finish. Note that depending on the version of STS / Eclipse, your version of Java, and other factors, you may encounter errors.  These will need to be fixed on a case-by-case basis. This may take a bit of time.

