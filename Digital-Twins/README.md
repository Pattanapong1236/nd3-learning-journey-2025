# 👯 Digital Twin & Virtual Engineering

การจำลองแบบทางวิศวกรรม (Engineering Simulation) และการสร้างคู่แฝดดิจิทัลเพื่อการวิเคราะห์พฤติกรรมระบบ

## 🧬 Digital Twin Architecture
องค์ประกอบทางเทคนิคของ Digital Twin แบ่งเป็น 3 ประเภท:
1.  **Digital Twin Prototype (DTP):** แบบจำลองก่อนการสร้างจริง (CAD, CAE, Finite Element Analysis)
2.  **Digital Twin Instance (DTI):** ข้อมูลของเครื่องจักรแต่ละเครื่องที่กำลังทำงานจริง (Operational Data)
3.  **Digital Twin Aggregate (DTA):** ข้อมูลรวมของเครื่องจักรทั้งระบบเพื่อวิเคราะห์ภาพรวม

## 🛠️ Virtual Commissioning (VC)
กระบวนการทดสอบระบบควบคุมกับแบบจำลองก่อนเดินเครื่องจริง เพื่อลด Lead Time และความเสี่ยง
* **MiL (Model-in-the-Loop):** ทดสอบ Logic กับ Mathematical Model (MATLAB/Simulink)
* **SiL (Software-in-the-Loop):** ทดสอบ Generated Code บน Virtual Controller
* **HiL (Hardware-in-the-Loop):** ทดสอบ PLC จริง เชื่อมต่อกับ Real-time Simulator ที่จำลองสัญญาณ Sensor/Actuator

## 🆔 Asset Administration Shell (AAS)
มาตรฐานการห่อหุ้มข้อมูล (Data encapsulation) ของสินทรัพย์อุตสาหกรรม (IEC 63278)
* **Concept:** AAS เปรียบเสมือน "USB Driver" ของเครื่องจักร ที่ทำให้ระบบอื่นๆ (ERP, Cloud) เข้าถึงข้อมูลและฟังก์ชันของเครื่องจักรได้ทันทีโดยไม่ต้องเขียน Driver ใหม่ (Plug-and-Produce)
* **Submodels:** เก็บรวบรวมข้อมูลจำเพาะ เช่น Technical Data, Documentation, Operational Status
