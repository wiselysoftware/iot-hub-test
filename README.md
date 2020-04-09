# Iot Hub communication Testing

These scripts are for connecting to an IoT Hub portal, using x509 certificates, based on the examples provided by Microsoft from the following repos:

[IoT Hub Samples](https://github.com/Azure-Samples/azure-iot-samples-node)

[Node SDK - IoT Hub Samples](https://github.com/Azure/azure-iot-sdk-node/tree/master/device/samples)

## Requirements

You need the latest or LTS version of Node.js currently being supported.
 

## Installation

In the device and client folder, after installing node, execute the following command:

```bash
$: npm install
```
You will also need to set the enviroment variables:
- DEVICE_CONNECTION_STRING (a string using the iothub and device name)
- PATH_TO_CERTIFICATE_FILE (path to the cert.pem file)
- PATH_TO_KEY_FILE (path to the cert.key file)
- KEY_PASSPHRASE_OR_EMPTY (a string with the passphrase)
- CONNECTION_STRING (The string used by the client for listening to messages)

It's also possible to just copy the variables directly on the scripts if having issues creating enviroment variables. Simply edit the code where the variables are being declared with the value (in the case of the certs, you have to include the line ----BEGIN CERTIFICATE--- and --- END CERTIFICATE--- in the strings)


## Use

After installation and configuration, in the corresponding folder, just execute:

```bash
$: node <file to run> 
```

where file to run should be either device or ReadDeviceToCloudMessages

## contact
If you have any questions, feel free to contact us at software@wisely.cl

