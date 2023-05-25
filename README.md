# **_Node-RED flow to send OpenWeatherMap(OWM) data to Fogwing_**

This repository contains a Node-RED flow, that allows you to retrieve weather data from the OpenWeatherMap API and send it to the Fogwing IoTHub API.

>**Note:** This Node-RED flow is specific to send OpenWeatherMap (OWM) to Fogwing. It may require additional modifications and configurations to work properly with your specific use case.

### Pre-requisites:
- [Node-RED](https://nodered.org/)

## **OpenWeatherMap to Fogwing Client Node-RED Flow**

To run the `flows.json` Node-RED flow, follow the step-by-step instructions below:

### **Step 1: Clone the Repository**
- Clone the [fogwing-thirdpatry-integration-node-red](https://github.com/factana/fogwing-thirdparty-integration-node-red/) repository containing the program code to your local machine.

### **Step 2: Install and run Node-RED**
- Install Node-RED on your local machine by following [this](https://nodered.org/docs/getting-started/) guide which provides detailed instructions on the installation process for a smooth setup.
- Once Node-RED is installed, open a Command Prompt or Terminal window and run the command node-red. Node-RED will start running and display log messages in the Command Prompt or Terminal window.
- Open a web browser and visit `http://localhost:1880` or `http://127.0.0.1:1880` to access the Node-RED editor interface  

### **Step 3: Import Flow**
- To import a flow file in Node-RED, open the editor interface and click on menu in the upper right corner of the window. Select Import from the menu and browse to the `flows.json` file from the downloaded file. Click on the Import button to import the flow into the editor.

### **Step 4: Update Credentials**
- Update your OpenWeatherMap API key and city name in the OWM Cred node.
- Update your Fogwing credentials with Fogwing Account ID, API key and Edge EUI in the FW Cred node.

>**Note:** Ensure that you provide valid OWM and Fogwing IoTHub credentials both nodes for successful data transmission.

### **Step 5: Run the Node-RED Flow**
- Click on **Send Data** node to send OWM data to Fogwing

>**Note:** If everything goes according to the instructions mentioned above, you should see OpenWeatherMap data and `{'statusCode': 201, 'message': 'Created', 'description': 'The Request Has Succeeded', 'data': 'Successfully published'}` message displayed in the Node-RED debug window. In case of any errors or issues, an error message will be shown instead.

### **Step 6. Analyze Your Data on the Fogwing Platform**
- Now you are ready to analyze your data at [Fogwing Platform](https://portal.fogwing.net/) portal, you can check all the data within the data storage in the portal.

## **Where to Find Help and Resources for Fogwing**
- [Fogwing Open APIs Docs.](https://api.fogwing.net/)
- [OpenWeatherMap API Docs.](https://openweathermap.org/api)
- [Fogwing Platform Forum.](https://community.fogwing.io/)
- [Fogwing Platform Docs.](https://docs.fogwing.io/)


## Please visit https://www.fogwing.io/industrial-iot-platform/ for more information about Fogwing Industrial IoT Platform. ##
