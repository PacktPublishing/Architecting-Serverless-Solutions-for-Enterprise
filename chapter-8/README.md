# IoT and Event Processing with IBM Cloud Functions ( OpenWhisk )

The purpose of this project is to collect temperature information send by an IoT sensor, persistently store them for future analysis, and also send out near-real-time alerts when the temperature crosses a specific threshold.

## Architecture

![Architecture Diagram](images/chapter8-project-v1.png)

## Pre-requisite

You should have an ibm cloud account to do this project.  It is assumed that you already have an account and can login to the cloud console at https://cloud.ibm.com/.  You should also setup the ibmcloud CLI following the instructions at the link:

[ Cloud CLI - getting started ](https://cloud.ibm.com/docs/cli?topic=cli-getting-started)

Once this CLI is setup, add the function plugin to it so that the cloudfunction/openwhisk cli would be available as a subcommand to ibmcloud CLI

[Cloud Functions CLI](https://cloud.ibm.com/functions/learn/cli)

## Project and sub tasks

The overall project can be broken down into following tasks

- [ Setup IBM Watson Platform Instance and add the device ]( WatsonIoT.md )
- [ Create Pseudo IoT device ]( PseudoIoT.md )
- [ Create the IBM Cloudant instance and database]( Cloudant.md )
- [ Create the consumer cloud function]( Consumer.md )
- [ Create the alerting cloud function]( Alerting.md )

Once these subtasks are completed, we proceed to use feeds to schedule the functions and test the pipeline end to end using the pseudo IoT device ( python script ).  Follow below instructions to complete the project.








