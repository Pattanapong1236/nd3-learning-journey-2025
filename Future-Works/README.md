# 🔭 Future Works & Engineering Roadmap

เอกสารฉบับนี้รวบรวมแผนแม่บททางวิศวกรรม (Engineering Roadmap) โครงการวิจัยและพัฒนา (R&D) และส่วนขยายระบบที่วางแผนไว้สำหรับอนาคต เพื่อยกระดับโรงงานสู่ระดับ **Autonomous Operations**

---

## 📅 Technology Roadmap Strategy
แผนยุทธศาสตร์การพัฒนาเทคโนโลยี แบ่งตามกรอบเวลาและความซับซ้อน

| Phase | Horizon | Focus Area | Engineering Goal |
| :--- | :--- | :--- | :--- |
| **Phase 1 (Short-term)** | 0-6 Months | **Visibility & Connectivity** | เชื่อมต่อเครื่องจักร Legacy ทั้งหมดเข้าสู่ระบบ (100% Data Acquisition) |
| **Phase 2 (Mid-term)** | 6-18 Months | **Prediction & Optimization** | นำ AI มาใช้ทำ Predictive Maintenance และจูน Parameter เครื่องจักรแบบ Real-time |
| **Phase 3 (Long-term)** | 18+ Months | **Autonomy (Dark Factory)** | ระบบตัดสินใจและแก้ไขปัญหาเองได้ (Self-optimizing & Self-healing) |

---

## 💡 Planned Projects (Future Initiatives)
รายละเอียดโครงการที่อยู่ในแผนงาน (Backlog) และรอการดำเนินการ

### 1. Project: 5G Private Network for AGV
**Objective:** ติดตั้งระบบเครือข่าย 5G ส่วนตัว (Private Network) เพื่อควบคุมรถขนส่งอัตโนมัติ (AGV) หลายคันพร้อมกันโดยไม่มีความหน่วง
* **Technical Scope:**
    * **Network:** ติดตั้ง 5G Small Cells ครอบคลุมพื้นที่ Warehouse 5,000 ตร.ม.
    * **Latency Target:** < 10ms (Ultra-Reliable Low Latency Communications - URLLC)
    * **Protocol:** เปลี่ยนการสื่อสารจาก Wi-Fi (Roamming ปัญหาเยอะ) เป็น 5G SIM-based
* **Expected ROI:** ลดเวลา Downtime ของ AGV จากปัญหาสัญญาณหลุดได้ 95%

### 2. Project: Closed-Loop AI Quality Control
**Objective:** สร้างระบบ QC ที่ "สั่งแก้เครื่องจักร" ได้เองทันทีเมื่อเจอของเสีย
* **Current Workflow:** กล้องเจอของเสีย -> แจ้งเตือน -> คนเดินมาปรับเครื่อง -> เริ่มใหม่
* **Future Workflow:** กล้องเจอของเสีย -> AI วิเคราะห์ -> **ส่งค่า Offset กลับไปที่ PLC** -> เครื่องปรับตัวเองทันที
* **Tech Stack:** Python (PyTorch), OPC UA (Write capability), Siemens S7-1500 PLC

### 3. Project: Blockchain for Supply Chain Traceability
**Objective:** ใช้ Blockchain เก็บข้อมูลการผลิตเพื่อส่งให้ลูกค้า (Automotive Tier 1) ตรวจสอบย้อนกลับ
* **Technical Scope:**
    * **Data:** เก็บ Serial Number, Torque Value, QC Result ของทุกชิ้นงาน
    * **Platform:** Hyperledger Fabric (Private Blockchain)
    * **Integration:** เขียน Smart Contract เพื่อรับข้อมูลจาก MES โดยอัตโนมัติ

---

## 🔬 Research & Development (R&D) Topics
หัวข้อเทคโนโลยีที่กำลังศึกษาความเป็นไปได้ (Feasibility Study)

### Time-Sensitive Networking (TSN)
* **Concept:** การทำให้เครือข่าย Ethernet ธรรมดา สามารถรับส่งข้อมูลแบบ Real-time ได้เหมือน Fieldbus ราคาแพง
* **Goal:** ศึกษาสวิตช์รุ่นใหม่ที่รองรับมาตรฐาน IEEE 802.1Qbv เพื่อรวม Traffic กล้องวงจรปิดและ PLC ไว้ในสายเส้นเดียวกันโดยไม่กวนกัน

### Edge AI Quantization
* **Concept:** การบีบอัด AI Model ขนาดใหญ่ ให้รันบนชิปราคาถูก (เช่น ESP32 หรือ Microcontroller)
* **Goal:** พัฒนา Sensor สั่นสะเทือนที่มี AI ฝังในตัว (TinyML) โดยไม่ต้องส่งข้อมูลดิบขึ้น Cloud เพื่อประหยัด Bandwidth

---
