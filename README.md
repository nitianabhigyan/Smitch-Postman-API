# Smitch-Postman-API
A postman collection to control switch smart devices.

Offical documentation for the Smitch Smart app control: [https://docs.developer.mysmitch.com](https://docs.developer.mysmitch.com)

## How to use
### Prerequisites
Please familiarise yourself with the basic prerequisite at: [Prerequisites](https://docs.developer.mysmitch.com/#0.-prerequisites)
<ul>
    <li>Register a developer account at: [Developer-Portal](https://developer.mysmitch.com) by selecting Sign Up (Sign In if you already created an account)
    <li>Add an App in your developer account and create a "TEST" API KEY. More details: [api-keys](https://docs.developer.mysmitch.com/app/api-keys). Save this api-key somewhere safe.
    <li>Link a "tester" to your application. More details: [user-tester](https://docs.developer.mysmitch.com/users/user-tester), make sure the tester's account used here is the same as the one you use to sign in the Smitch mobile app.
</ul>

### Using the collection.

<ol>
    <li>Load the collection in your Postman.
    <li>Open the "Smitch Postman API collection", select the variables tab and set the "api_key" variable's value to your api_key obtained from.
    <li>Select the "Everything_is_valid" request and send it. If everything was done correctly, this should return a  "status": "success". If not, please validate your steps again.
    <li>Select the "list_of_users" request and send it. Obtain the user_id variable of the desired user (make sure the said account is added as tester as per above), add this key's value to your collection's variable "user_id" variable's value.
    <li>To control a device, you first need to identify it's "device_id" and add it in collection's variables. To obtain a list of all devices added in user's account please use the "get_user_details" request.
</ol>
