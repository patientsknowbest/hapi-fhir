HAPI FHIR
=========

HAPI FHIR - Java API for HL7 FHIR Clients and Servers

Complete project documentation is available here:
http://jamesagnew.github.io/hapi-fhir/

A demonstration of this project is available here:
http://hapi.fhir.org/

This project is Open Source, licensed under the Apache Software License 2.0.

Please see [this wiki page](https://github.com/jamesagnew/hapi-fhir/wiki/Getting-Help) for information on where to get help with HAPI FHIR. Please see [Smile CDR](https://smilecdr.com) for information on commercial support.

## PKB artifact

Some minor changes were made to the original branch for the hapi-fhir-validation-resources-dstu3 project.
Steps to deploy this artifact:
- clone repository
- change artifact version if needed: `mvn versions:set -DnewVersion=3.8.0-PKB`
- install to check it's working: `mvn install -DskipTests -pl hapi-fhir-validation-resources-dstu3 -am`
- deploy to GH: `mvn deploy -DaltDeploymentRepository=<ID-from-settings.xml>::default::<URL-to-deploy-to>`
