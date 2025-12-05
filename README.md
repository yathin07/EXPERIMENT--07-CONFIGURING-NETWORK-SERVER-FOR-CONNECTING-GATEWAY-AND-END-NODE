# EXPERIMENT -07 CONFIGURING NETWORK SERVER FOR CONNECTING GATEWAY AND END NODE 
**NAME: Yathin Reddy T**
**ROLL NO: 212223100062**
**DEPARTMENT: CSE(CS)**
## Aim: 
To  configure the Network server and end device for transferring data on the network
## Components required: 
End node stm 32 development kit , Dragino LPS8, Network server 

## Theory :
When working with sensitive applications or files, saving progress on your local device is a start, but what if you lose access to your device? Network servers address this problem by hosting the files and programs most pertinent to the network and enabling access for consistent, real-time use. 

As a result, personnel or network clients can instantly access important data or tools while also facilitating collaboration between users. Multiple users can make changes to the same program or document for continued development over the course of a project. Via a secure login, remote users can connect to the home network.
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/59db9b76-ddd5-4d6a-9075-8db233f5e479)


In the above graphic, the circle represents an organization network where a network server facilitates collaboration and file sharing between network clients (devices).

 The role of a network server, then, is to provide users with a set of services and access to resources on the network. These features include:

Permissioned access and log-ins for network users Gateway access to the Internet for an organization Centralized location for network resources  Shared access to devices on the network like a printer or a scanner Hosts multi-user apps like email servers, web applications, or CRM

## Procedure :

 1. login to the network server using login link  https://iot.saveetha.in/
 2. Click on the nework server
  
 3. Click on the add gateway 
 <img width="1662" height="954" alt="image" src="https://github.com/user-attachments/assets/70c772bb-d23d-4f1e-ad0e-0229a0ba6556" />

4. Click on the lora options , lora - frequency plan 
<img width="1491" height="928" alt="image" src="https://github.com/user-attachments/assets/0e671a7a-a7cb-448a-a270-79f00e73662b" />

5. Click on devices then click add

6. Add the attributes in the end device as  shown below 

<img width="1593" height="1009" alt="image" src="https://github.com/user-attachments/assets/0020ac85-f28e-441d-9478-aa8da48bedd5" />

7.Using AT commands configure end device in serial port utility
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
<img width="1631" height="980" alt="image" src="https://github.com/user-attachments/assets/b547b70e-5446-40bd-8205-e936ebcb541c" />




## Result: 

  The Network server and end device for transferring data on the network has been accomplished.
