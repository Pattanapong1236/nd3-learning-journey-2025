# 🧠 Industrial Data Analytics & Machine Learning

สถาปัตยกรรมกระบวนการจัดการข้อมูล (Data Pipeline Architecture) และการประยุกต์ใช้ AI ในงานวิศวกรรม

## 🌊 Data Pipeline Architecture
การออกแบบ Flow ข้อมูลสำหรับ High-Frequency Industrial Data

1.  **Ingestion:** การรับข้อมูลจาก Edge Gateway (รองรับ Protocol Modbus/OPC UA)
2.  **Time-Series Database (TSDB):** การจัดเก็บข้อมูลที่มี Timestamp เป็น Key หลัก (InfluxDB, TimescaleDB) เพื่อรองรับ High Write Throughput
3.  **Processing (Edge vs Cloud):**
    * *Edge Analytics:* การประมวลผลเบื้องต้นที่ Gateway (เช่น การกรอง Noise, Downsampling)
    * *Cloud Computing:* การเทรนโมเดลขนาดใหญ่

## 🔍 Signal Processing & Predictive Maintenance (PdM)
เทคนิคทางวิศวกรรมในการวิเคราะห์สัญญาณเพื่อทำนายความเสียหาย

* **Vibration Analysis:** การใช้ **FFT (Fast Fourier Transform)** แปลงสัญญาณการสั่นสะเทือนจาก Time Domain เป็น Frequency Domain เพื่อหาความถี่ผิดปกติ (Fault Frequencies) ของตลับลูกปืน (Bearing Faults) หรือการเยื้องศูนย์ (Misalignment)
* **Current Signature Analysis (MCSA):** การวิเคราะห์สัญญาณกระแสไฟฟ้าของมอเตอร์เพื่อตรวจจับความผิดปกติของ Rotor Bar

## 🤖 ML Model Deployment
* **Anomaly Detection:** การใช้ Unsupervised Learning (เช่น Autoencoders, Isolation Forest) เพื่อตรวจจับความผิดปกติที่ "ไม่เคยเกิดขึ้นมาก่อน"
* **Model Serving:** การแปลง Model เป็น ONNX Format หรือใช้งาน TensorFlow Lite เพื่อรันบน Edge Devices (Industrial PC / Raspberry Pi)
