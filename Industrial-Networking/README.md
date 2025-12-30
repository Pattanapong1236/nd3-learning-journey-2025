# 🌐 Industrial Communication & Network Architecture

รายละเอียดทางเทคนิคของสถาปัตยกรรมเครือข่ายอุตสาหกรรม การบรรจบกันของ OT/IT และมาตรฐานการรับส่งข้อมูล



## 🔺 The Automation Pyramid (Purdue Model)
มาตรฐานการแบ่งเลเยอร์เครือข่ายเพื่อความปลอดภัยและการจัดการข้อมูล (ISA-95)

* **Level 0 (Field):** Sensors, Actuators, Instrumentation (4-20mA, IO-Link)
* **Level 1 (Control):** PLC, DCS, PID Controllers (Real-time critical, Latency < 10ms)
* **Level 2 (Supervisory):** SCADA, HMI (Monitoring & Control)
* **Level 3 (MOM/MES):** Manufacturing Execution Systems (Batch management, Scheduling)
* **Level 4 (Enterprise):** ERP (Business Logistics)

## 📡 Industrial Protocols Specification

### OPC UA (Open Platform Communications Unified Architecture)
มาตรฐานหลักสำหรับการทำ **Semantic Interoperability** (IEC 62541)
* **Architecture:** Client-Server และ Pub/Sub (over UDP)
* **Information Modeling:** การนิยามโครงสร้างข้อมูลเชิงวัตถุ (Object-Oriented) ไม่ใช่แค่ Raw Data
* **Security:** Built-in X.509 Certificate Authentication & Encryption

### MQTT (Message Queuing Telemetry Transport)
โปรโตคอลสำหรับ IIoT ที่เน้น Bandwidth Efficiency
* **Implementation:** ใช้ **Sparkplug B** Payload Specification เพื่อกำหนดโครงสร้างข้อมูลมาตรฐานสำหรับงานอุตสาหกรรม (ป้องกันปัญหา Data Inconsistency)
* **QoS Levels:** ใช้ QoS 1 หรือ 2 สำหรับข้อมูล Critical Alarms

### Fieldbus vs Industrial Ethernet
* **Determinism:** Industrial Ethernet (Profinet, EtherCAT, Ethernet/IP) ถูกออกแบบมาให้มีความแน่นอนของเวลา (Low Jitter) ต่างจาก Ethernet สำนักงาน (TCP/IP) ที่เป็น Best Effort

## 🛡️ Network Security & Topology
* **Design:** ใช้โครงสร้างแบบ **Ring Topology** (RSTP/MRP) เพื่อทำ Redundancy ในระดับ Layer 2
* **Segmentation:** การทำ VLAN แบ่งแยก Traffic ระหว่าง Machine Network และ Office Network
* **DMZ (Demilitarized Zone):** การตั้ง Industrial Gateway กั้นกลางระหว่าง OT และ IT เพื่อป้องกันการเข้าถึงโดยตรงจากภายนอก
