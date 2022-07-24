# Networking

## NMS
- Network Management System
- It act like as a eyes of Network  
- NMS can manage a complete Networks(Multiple Networks/Vendors)
- NMS has all functionalities of EMS
- NMS can manage number of EMS es
- NMS can able to Understand Inter-Relationship between Devices/Nodes/Elements
- NMS can provide **Co-related alarms** among Nodes/Elements also provides the **Root Cause**
- **Protocals**
  - SNMP
  - JMX
- **Examples**
  - PRTG
  - ZABBIX
  - Open NMS
  - Nagios


## EMS
- Elements Management System
- EMS can manage Only 
  - single Node/Network/Element 
  - same group of Nodes/Network/Elements
- EMS can not able to understand Inter-Relationship between Deevices/Nodes/Elements
- EMS can provide individual **alarms** but not root cause
- **Protocals**
  - SNMP
  - CORBA
  - XML

## SNMP
- Simple Network Management Protocal
- Internet Standard Protocal
- Widely famous for Network Monitoring
- SNMP will collect & organize the **Information** of Managed Devices on IP Networks
- Versions
  - SNMPv1
  - SNMPv2c(commercial) -Updated with more reliable and security features
  - SNMPv3              -Improved Privacy, Authentication

## TMN Architecture
- Telecommunication Management Network

- **TMN Hierarchy**
1. NE layer
  - It Defines Interface for Network Elements
  - Ideally Covering all FCAPS areas
2. Element Management Layer
3. Network Management Layer
4. Service Management Layer
5. Business Management Layer


## FCAPS
- Fault Management
- Configure Management
- Accounting Management
- Performance Management
- Security Management


## MIB
- Management Information Base
- The formate of MIB is defined as part of **SNMP**
- MIB is a SNMP flat-file, nonrelational database that describe devices being monitored.
- **Components**
  - Address
    - Specify the Address
    - **Ex** 135.254.214.63
  - Advanced
    - Address
    - Port(by Defult: **161**)
    - Read Community
    - Write Community
    - SNMP Version (Present Version **V2**)
  - OID
    - Object Indentifiers
    - OID uniquely Identify managed objects in a MIB hierarchy
  - Operations
    - Get Next
    - Get
    - Get Bulk
    - Get Subtree
    - Walk
    - Set
  - SNMP MIBs
    - MIB Tree
    - Attributes
    - Read-Only(**ro**) Represents as Leaf
      - Set Operation Doesn't work here
    - Read-Write(**rw**) Represents as Pen
      - Set Operation Work here
  - Result Table
    - Name/OID
    - Value
    - Type
    - IP:Port


## TCP/IP


## ISO/OSI
- **OSI** - Open System Interconnection
- **ISO** - International Organization of Standardization


## Network Layers
- **Application Layers**
  - This is 7th Layer in OSI Model
  - Input & OutPut of Data
  - Sending & Recieving Data
  - Network Applications
    - **EX** Chrome, Mozrilla, Outlook, Skype, etc.,
  - It will depends on Application Layer Protocals
  - **FTP** - File Transfer Protocal
    - File Transfer
  - **HTTP & HTTPS** - Hyper Text Transfer Protocal Secure
    - Web Surfing
  - **SMTP** - Simple Mail Transfer Protocal
    - Emails @
  - **Telnet** - Tele Type Network
    - Virtual Terminals

- **Presentation Layers**
  - It takes data from Application Layer
  - It specifies the architecture for independent data transfer
  - It encodes & decodes the data
  - It Compress & Decompress the data
  - It encyrpts & decrypts the data
  - **SSL** - Secure Socket Layer Portcal
    - Used for Encryption & Decryption

- **Session Layers**
  - It manages and controls user session & Dialougs
  - It reports the upper layer errors
  - here only host communication is processed
  - No protocals involved in this session layer
  - Files are received in tha Data Packets Formate
  - This layer helps in session management and Authentication.

- **Transport Layers**
  - It manages end to end message delivery in network by giving acknowledgement to users
  - It provides Sequential packets delivery through error recovery and flow control mechanisms
  - It provides Connection less oriented packet delivery
  - Multiplexing and segmenting done here
  - This layer involves in Segmenting, Flow control & error control
  - Segmenting contains Port & Sequence numbers and this Numbers helps to connecting to the Applications(Chrome, Mozila)
  - It performs two types of services:
  1. Connection oriented transmission done via TCP(Transimission control protocol)
  2. Connectionless transmission done via UDP(User datagram protocol)
  
- **Network Layers**
  - Data devided in to Packets
  - It determines the data transfer mechanism between network devices
  - It determines the path for flow control of data
  - IP(Internet protocol) & Router are involved in this layer
  - IP addressing(IPv4 & IPv6) is done in this layer called Logical addressing
  - 

- **Data Link Layers**

- **Physical Layers**
