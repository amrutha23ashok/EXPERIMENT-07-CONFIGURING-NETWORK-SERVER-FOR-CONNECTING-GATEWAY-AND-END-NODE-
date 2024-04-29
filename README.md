 ### EXPERIMENT -07 CONFIGURING NETWORK SERVER FOR CONNECTING GATEWAY AND END NODE 
 
## Aim: To  configure  the Network server and end device for traferring data on the network
## Components required: end node stm 32 development kit , dragino LPS8, network server 

## Theory :
When working with sensitive applications or files, saving progress on your local device is a start, but what if you lose access to your device? Network servers address this problem by hosting the files and programs most pertinent to the network and enabling access for consistent, real-time use. 

As a result, personnel or network clients can instantly access important data or tools while also facilitating collaboration between users. Multiple users can make changes to the same program or document for continued development over the course of a project. Via a secure login, remote users can connect to the home network.
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/59db9b76-ddd5-4d6a-9075-8db233f5e479)


In the above graphic, the circle represents an organization network where a network server facilitates collaboration and file sharing between network clients (devices).

 The role of a network server, then, is to provide users with a set of services and access to resources on the network. These features include:

Permissioned access and log-ins for network users Gateway access to the Internet for an organization Centralized location for network resources  Shared access to devices on the network like a printer or a scanner Hosts multi-user apps like email servers, web applications, or CRM

## Procedure :

 1. login to the network server using login link  https://iot.saveetha.in/
 2. Click on the nework server as shown blow 
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1bd434ca-1426-4102-8384-94473483543e)
 3. click on the add gateway 
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/47c2e08d-6598-4437-8b07-f213d6f3b8ac)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/e62ff028-99bc-485e-9808-fbb6e124f8b2)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/a2e3ae58-6402-49e8-8f96-679059c1842c)
4. click on the lora options , lora - frequency plan 
5. click on channel s and create a new channel after which you can add a new end device 
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1fb72be5-e48d-4cde-a329-0cfb0d29070f)
6. add the attributesin the end device as  shown below 
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/00bff30b-42fc-42d5-9540-285d270e41cb)
7.using AT commands configure end device in serial port utility
AT Commands to set initially (Mandatory)
 AT+FDR // To do factory data reset
 AT+NJM=1 // To set OTAA mode
 AT+ADR=1 // To enable the ADR
 AT+TDC=600000 // To set the default sampling interval as 10 minutes
(Should not give below 5 minutes)
 AT+CLASS=C // To set class C
 AT+DEUI=XX XX XX XX XX XX XX XX // To set Device EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX // To set APP EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX //
To set APP Key
 ATZ // To take effective action on below settings (As like saving)



## OUTPUT 

![image](https://github.com/amrutha23ashok/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/120772913/902cb0ac-6e98-4812-905e-dac7369d1907)

![image](https://github.com/amrutha23ashok/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/120772913/276b0e6f-2aa1-4114-b4ad-129064fc4e8f)

![image](https://github.com/amrutha23ashok/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/120772913/d7024842-0176-4b59-93c9-f8b033d35053)
![image](https://github.com/amrutha23ashok/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/120772913/8e72235c-cd61-4242-8e7a-f7096e4b91ec)
![image](https://github.com/amrutha23ashok/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/120772913/69fd3360-a730-4f91-a3a6-2dc75badc236)
![image](https://github.com/amrutha23ashok/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/120772913/bdd19d12-83ed-4806-a5be-bf246c9afe48)

![image](https://github.com/amrutha23ashok/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/120772913/16d09554-60da-4bfc-b95c-7ba5fc1f0485)
![image](https://github.com/amrutha23ashok/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/120772913/96edd83f-56fd-4d4e-b096-b79859a084ed)




## Results: 

  The Network server and end device for traferring data on the network has been accomplished.

