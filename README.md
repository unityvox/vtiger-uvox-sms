# UVox & Vtiger SMS Notified.

**About The API**
The UVox API provides a simple but powerful interface that allows you to integrate your own applications with the UVox services. An extensive set of actions can be performed using this API, such as sending SMS, Checking Balance, Checking call rates, Supplying QR Codes for Softphone, Vtiger CRM Integration and other operational data. As such, this interface is the ideal tool for creating alternative dashboards, developing mobile applications and automating front-end and back-end applications.

The UVox API is a fully compatible implementation of the JSON API specification, which defines how an application should request that resources be retrieved or modified, and how a server should respond to those requests. This REST (Representational State Transfer) interface provides an easy-to-use set of HTTP endpoints that allow you to access our services using the GET, PUT, POST methods.

THIS DOCUMENT ASSUMES THAT IT IS FAMILIAR WITH THE CONCEPTS OF WEB PROGRAMMING, THE FORMATS OF WEB DATA AND WITH THE SPECIFICATION OF THE JSON API. ADDITIONAL INFORMATION ABOUT JSON IS AVAILABLE ON YOUR OFFICIAL WEBSITE.

[UVox | IP Communications](https://unityvox.com)

This feature gives you the flexibility to send text messages to your customers. You can send text messages to multiple records in one shot. In addition to manually sending messages, you can also send automatic notifications activated by workflows in Vtiger CRM. 

## Install Console

```
cd /var/www/html/vtigercrm/modules/SMSNotifier/providers

wget  https://github.com/unityvox/vtiger-uvox-sms/blob/master/UVox.php

```
## Install FTP

[Download](https://github.com/unityvox/vtiger-uvox-sms/blob/master/UVox.php)

save the content via FTP in /path CRM Vtiger/modules/SMSNotifier/providers

- Click on the SMS Notifier tab. You can find it in All the drop-down menus in the menu bar.
- Click on the wrench icon> Server configuration
- Click on New configuration and configure the following details in the pop-up window that appears.

Complete all the information requested in the form.

<img src="https://unityvox.com/assets/web/images/vtiger_1.png">

- **Provider** = We select UVox from the drop-down list.
- **Active** = We set the activation of the service to yes.
- **User Name** = Your registered email in our systems when creating your account in UVox.
- **Password** = Password for your account at my.unityvox.com
- **Accountnumber** = Account number, you can find it in your administration panel in the API Key section.
- **Apikey** = Private key generated in your account https: /my.unityvox.com.
- **From** = Phone number that sends the SMS, some operators and mobile teams accept text as recipient, you can place your name, Ej from = "UVox", if you place a text and the operator does not accept it the recipient will be a generic number. Some countries do not support labels so the sender will be a generic number.

We save the form, we have already configured our Gateway to send SMS

<img src="https://unityvox.com/assets/web/images/vtiger_2.png">

**SMS sending**


To send SMS to records in the list view. 

- Click on the desired module. For example, contacts, contacts or organizations. 
- Select the desired records to which you want to send SMS. You can select records by clicking on the corresponding boxes that precede the records.

<img src="https://unityvox.com/assets/web/images/vtiger_3.png">

- Now click on the Actions> Send SMS' drop-down menu

<img src="https://unityvox.com/assets/web/images/vtiger_4.png">

- Select the field where the mobile numbers of your contacts are stored.

<img src="https://unityvox.com/assets/web/images/vtiger_5.png">

<img src="https://unityvox.com/assets/web/images/vtiger_6.png">


## Problemas / Contribuciones 
Found a bug or missing a feature? Log it [here](https://github.com/unityvox/vtiger-uvox-sms/issues) and we will take a look.
