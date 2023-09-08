# Computer Networks

> 车啸平

* 考核
  * 5% Class Practice
  * 45% Assignments
    * we'll do homework on friday (biweekly)
  * 50% Final Examination (Open Book)

* References
  * 要买: Computer Networking: A Top-Down Approach (7th)

* A mini game about communication

* 16 Weeks Plan

## 1. Introduction

* Networks Model
  * Client-Server Model
  * Peer-to-peer

* Rules <=> Protocols

* Protocol layers
  * main structuring method used to divide up netowrk funcitonality
  * each protocol at different layerse serves a different purpose

* wireless vs mobile

* Networks
  * PAN: Personal Area Network
  * LAN: Local Area Network (Enterprise Network)
  * MAN: Metropolitan Area Network
  * WAN: Wide Area Network

* Internet Service Provider
  * ISP provide WAN
  * Tier-1 ISP, Tier-2 ISP, ..., Local ISP, BJTU Network
  * China have only **2 Tier-1 ISP**: CN-China Telecom, CN-CHina Unicom
  * 为什么要分级：每个设备支持数量有限

* CDN

* VPN: Virtual Private Network
  * have the right to **go inside LAN**

* Internet

* Q1: 不是所有的网站都需要Internet
  * 同个LAN下的网站就不需要

* Q2: 可以用无线方法连接多个Router吗

* Q3: 使用ISP连接Internet

* History of Chinese Internet

* Social Issues of Internet

* Reference Model
  * OSI Reference Model
    * 7 Levels
      1. Physical     : sends bits as signal
      2. Data link    : sends frames (todo)
      3. Network
      4. Transport
      5. Session
      6. Presentation
      7. Application
  * TCP/IP Reference Model
    * 5 Levels
      1. Physical
        * Bit (0 or 1)
      2. Link
        * Frame (1010100101)
      3. Network
        * Packet
      4. Transport
        * Segment
      5. Application
        * Message
    * 信息来自应用层，并往下传递，每传递一层，会多一个**Header**
    * Router 会处理 physical, link, network
    * Switch 只处理 physical, link
    * 例，浏览器每个层使用的协议为: HTTP, TCP, IP, 802.11
      * 802.11 是 Wifi 的协议
      * 802.3 是 以太网(Ethernet) 的协议
    * 不同层有不同的协议，每个协议都有自己的Header格式
    * 一条信息，发送和接收使用的协议必须相同
