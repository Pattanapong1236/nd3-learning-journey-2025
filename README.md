# nd3-learning-journey-2025

> **Description:** ฐานความรู้และโครงการพัฒนาระบบอัตโนมัติอุตสาหกรรม (Industrial Automation) เพื่อรองรับนโยบาย Thailand 4.0 โดยเน้นการบูรณาการเทคโนโลยี IIoT, Digital Twins และ AI เข้ากับกระบวนการผลิตจริง

![Status](https://img.shields.io/badge/Status-Active-success)
![Industry](https://img.shields.io/badge/Industry-Manufacturing%20%7C%20EEC-blue)
![Tech Stack](https://img.shields.io/badge/Tech-PLC%20%7C%20SCADA%20%7C%20Python-orange)

---

## 📑 สารบัญ (Table of Contents)

1. [Thailand’s Industrial Automation](#-thailands-industrial-automation)
2. [Industrial Networking and IoT](#-industrial-networking-and-iot)
3. [Digital Twins](#-digital-twins)
4. [Data Processing and Machine Learning](#-data-processing-and-machine-learning)
5. [Future Works/Projects](#-future-worksprojects)

---

## 🏗️ Thailand’s Industrial Automation

บริบทและทิศทางของอุตสาหกรรมไทยในการเปลี่ยนผ่านสู่ Smart Factory (Industry 4.0)

> 📂 **Documentation:** [ดูข้อมูลเจาะลึกในโฟลเดอร์ Thailand Industry](./thailand-industry/README.md)

* **Thailand 4.0 Policy:** การยกระดับอุตสาหกรรมในพื้นที่ EEC (Eastern Economic Corridor) สู่ S-Curve Industries (ยานยนต์สมัยใหม่, อิเล็กทรอนิกส์อัจฉริยะ)
* **Automation Landscape:** การเปลี่ยนผ่านจากแรงงานคน (Labor Intensive) สู่ระบบอัตโนมัติและหุ่นยนต์ (Robotics & Automation)
* **Key Challenges:** การขาดแคลนบุคลากร (Talent Gap), การอัปเกรดเครื่องจักรเก่า (Retrofitting Legacy Machines), และความคุ้มค่าในการลงทุน (ROI Analysis)

---

## 🌐 Industrial Networking and IoT

โครงสร้างพื้นฐานเครือข่ายอุตสาหกรรมและการเชื่อมต่ออุปกรณ์ (OT/IT Convergence)

> 📂 **Documentation:** [ดูข้อมูล Protocols และ Network ในโฟลเดอร์ Industrial Networking](./industrial-networking/README.md)

* **OT Protocols (Operational Technology):**
    * *Modbus TCP/RTU:* มาตรฐานพื้นฐานสำหรับการสื่อสารระหว่าง PLC และ Sensor
    * *OPC UA:* มาตรฐานกลางสำหรับการแลกเปลี่ยนข้อมูลที่ปลอดภัยและเป็นอิสระจากผู้ผลิต (Platform Independent)
* **IIoT Protocols (Industrial IoT):**
    * *MQTT:* สำหรับส่งข้อมูลจาก Edge Gateway ขึ้นสู่ Cloud/Dashboard
* **Network Topology:** การออกแบบวงจร Ring/Star เพื่อความเสถียร (Redundancy) และการแบ่ง Zone (VLAN) เพื่อความปลอดภัย

---

## 👯 Digital Twins

การจำลองคู่แฝดดิจิทัลเพื่อการวิเคราะห์และจำลองสถานการณ์

> 📂 **Documentation:** [ดูข้อมูลการจำลองระบบในโฟลเดอร์ Digital Twins](./digital-twins/README.md)

* **Virtual Commissioning:** การจำลองการทำงานของเครื่องจักรและดีบักโค้ด PLC บน Software ก่อนเดินเครื่องจริง (ลดความเสี่ยงและความเสียหาย)
* **Asset Administration Shell (AAS):** มาตรฐานการสร้างโมเดลข้อมูลของเครื่องจักรเพื่อการแลกเปลี่ยนข้อมูลที่เป็นสากล
* **Simulation Tools:** การใช้งานโปรแกรมจำลอง (เช่น Siemens NX, Matlab Simulink) เพื่อจำลองพฤติกรรมทางฟิสิกส์

---

## 🧠 Data Processing and Machine Learning

การนำข้อมูลการผลิตมาวิเคราะห์เพื่อเพิ่มประสิทธิภาพและลด Downtime

> 📂 **Documentation:** [ดูข้อมูล Data Pipeline และ AI Model ในโฟลเดอร์ Data ML](./data-ml/README.md)

* **Industrial Data Analytics:**
    * *OEE (Overall Equipment Effectiveness):* การคำนวณประสิทธิผลโดยรวมของเครื่องจักรแบบ Real-time
* **Predictive Maintenance (PdM):**
    * การใช้ Machine Learning (Regression/Classification) วิเคราะห์ค่าการสั่นสะเทือน (Vibration) และอุณหภูมิ เพื่อทำนายการชำรุดของมอเตอร์ล่วงหน้า
* **Computer Vision in QC:** ระบบตรวจสอบคุณภาพสินค้าอัตโนมัติด้วย AI Image Processing

---

## 🚀 Future Works/Projects

แผนงานโครงการและการพัฒนาเทคโนโลยีในอนาคต

> 📂 **Documentation:** [ติดตามสถานะโปรเจกต์ในโฟลเดอร์ Projects](./projects/README.md)

- [ ] **Legacy Machine Retrofit:** ติดตั้ง IoT Gateway ให้เครื่องจักรเก่า (CNC) ส่งข้อมูลผ่าน OPC UA ได้
- [ ] **Energy Monitoring System:** ระบบติดตามการใช้พลังงานไฟฟ้าในไลน์การผลิตเพื่อลดต้นทุน
- [ ] **AI-Driven Quality Control:** พัฒนาโมเดล Deep Learning ตรวจจับรอยขีดข่วนบนชิ้นงานโลหะ
- [ ] **Real-time Digital Twin Dashboard:** สร้างหน้าจอ 3D แสดงสถานะเครื่องจักรจริงผ่าน Web Browser
