# Basic ACD Custom Processor

This custom nifi processor is a simple ACD (Annotator for Clinical Data) handler that will take a string of text and
via a call to ACD, create flowfiles corresponding to any resources (medications or procedures)
that are found in the response.

## To build this artifact

### Prerequisites

The following must be installed on your system:

- maven
- java 8 or higher

### Steps

1. Navigate to the the nifi-acd-processor-bundle directory
1. Perform the build with `mvn clean install`
1. Navigate to the nifi-acdprocessors-nar/target directory. The .nar file should be present.  
1. Copy the .nar file to your nifi implementation, either into the library folder or into the extensions folder
