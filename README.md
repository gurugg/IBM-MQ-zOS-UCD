# IBM UrbanCode Deploy MQ z/OS - Generate MQSC Commands Plugin [![Build Status](https://travis-ci.org/IBM-UrbanCode/IBM-MQ-zOS-UCD.svg?branch=master)](https://travis-ci.org/IBM-UrbanCode/IBM-MQ-zOS-UCD)
---
Note: This is not the plugin distributable! This is the source code. To find the installable plugin, go into the 'Releases' tab, and download a stable version.

### License
This plugin is protected under the [Eclipse Public 1.0 License](http://www.eclipse.org/legal/epl-v10.html)

### Overview

The IBM MQ for z/OS – Generate MQSC Commands plugin can be used to provision IBM MQ for z/OS queue and channel resources. Resources are represented in REST form, held in files in a Source Control Management (SCM) system, and deployed to a target IBM MQ for z/OS queue manager environment.

View the doc folder for additional white paper documentation and sample triplet files.

### Steps:

    Generate MQSC Commands

### Compatibility
This plug-in is supported to run with IBM z/OS V2.1 (or later) and IBM MQ for z/OS V7.1 (or later). However, as the end of service (EOS) date for IBM MQ for z/OS V7.1 is 6th Nov, 2017, it is recommended that IBM MQ for z/OS V8 (or later) be used. As the plugin generates MQSC commands from the REST form resource representations, it is important to ensure that the generated MQSC is supported by the version of IBM MQ for z/OS in use. The list of supported MQSC attributes for queue and/or channel resources can be found in the IBM MQ for z/OS Knowledge Center specific to the version of IBM MQ for z/OS in use. Attempts to use unsupported MQSC attributes will result in a failure of the MQSC command on the target MQ for z/OS queue manager environment.

This plug-in requires version 6.2.2 (or later) of IBM UrbanCode Deploy.

### Installation
	The packaged zip is located in the 'Releases' tab. No special steps are required for installation.
	See Installing plug-ins in UrbanCode Deploy. Download this zip file if you wish to skip the
	manual build step. Otherwise, download the entire MQ-zOS-UCD and
	run the "ant" command in the top level folder. This should compile the code and create
	a new distributable zip within the '/releases' folder. Use this command if you wish to make
	your own changes to the plugin.

### History
    Version 1
        Initial beta release
