# RADIUS TASK#1 DOCS


## Table of Contents
* [Summary](#summary)
* [Example](#Example)

<a name="summary"></a>
## Summary
This task inteded to install, configure RADIUS on cloud VM and add usage policy on auth*ed users.

The **status of this task** can be found [HERE](https://trello.com/b/XNf6XnMI)

<a name="Example"></a>
## Example
### Follow this guied to add auth* ability to your NAS device (Home Gateway for example).

### Steps
1. Login to router configuration page

    <img src="./images/1.png" alt="drawing" width="300"/>

2. Under WLAN setting change to the following configuration:
    ```bash
    1. Security: 'WPA-EAP/WPA2-EAP'
    2. RADIUS server address: '165.22.16.207'
    3. RADIUS server port: '1812'
    4. RADIUS shared key: 'testing123'
    ```
    <img src="./images/2.png" alt="drawing" width="500"/>

3. Click `Submit` and you can reboot your router 

4. On any mobile device open WIFI settings and choose the network name.

    <img src="./images/3.png" alt="drawing" width="300" height="500"/>
5. Change the following configuration:
    ```bash
    EAP method: 'PEAP'
    CA certificate: 'Do not validate'
    Identity: 'omara'
    Password: 'hoopeo'
    ```
    <img src="./images/4.png" alt="drawing" width="300" height="500"/>
    
    then click `conntect`

Now your device should be connected to the Internet. If not consult your network adminstrator :)
