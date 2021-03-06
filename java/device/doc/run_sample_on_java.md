# Getting started - running a Java sample application

This "Getting Started" document shows you how to build and run any of the samples contained within the samples folder. 

## Prerequisites

Before you get started, you should:
- [Prepare your development environment][devbox-setup]
- [Setup your IoT Hub][setup-iothub]
- Configure your device in IoT Hub. <br/>See the section "Configure IoT Hub connection" in the document [How to use Device Explorer][device-explorer].

## Build and run the samples

If you have successfully [prepared your development environment][devbox-setup] the IoT device SDK and all samples should be built and ready to use. 

1. Start a new instance of the [Device Explorer][device-explorer], select or create a new device, obtain and note the connection string for the device, and begin moitoring under the Data tab.

2. Navigate to the folder containing the executable JAR file for the sample that you wish to run and run the samples as follows:

	The executable JAR file for sending event
	can be found at:
	
	```
	{IoT device SDK root}/java/device/samples/send-event/target/send-event-{version}-with-deps.jar
	```
	
	Navigate to the directory with the event sample. Run the sample using the following command:
	
	```
	java -jar ./send-event-{version}-with-deps.jar "{connection string}" "{number of requests to send}" "{https or amqps}"
	```
	
	The executable JAR file for receiving messages can be found at:
	
	```
	{IoT device SDK root}/java/device/samples/handle-messages/target/handle-messages-{version}-with-deps.jar
	```
	
	Navigate to the directory with the messages sample. Run the sample using the following command:
	
	```
	java -jar ./handle-messages-{version}-with-deps.jar "{connection string}" "{https or amqps}"
	```
	
	Note that the double quotes around each argument are required.


## Documentation

The documentation can be found at:

<!-- This path will need to be updated with the new api docs folder path -->
```
{IoT device SDK root}/java/device/iothub-java-client/doc/iothubclient_java_library/index.html
```

_In the future, the documentation will have a dedicated URL._

[devbox-setup]: devbox_setup.md
[setup-iothub]: ../../../doc/setup_iothub.md
[device-explorer]: ../../../tools/DeviceExplorer/devdoc/how_to_use_device_explorer.md