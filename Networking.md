# Networking
## NMS
- Network Management System
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

## FCAPS
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
    - Read-Only(ro) Represents as Leaf
      - Set Operation Doesn't work here
    - Read-Write(rw) Represents as Pen
      - Set Operation Work here
  - Result Table
    - Name/OID
    - Value
    - Type
    - IP:Port
## TCP/IP
## ISO/OSI
## Network Layers