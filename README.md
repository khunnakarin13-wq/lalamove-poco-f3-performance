# 🚀 Lalamove Performance Preset v2.4-max (Aggressive + Safe)

**สำหรับ POCO F3 (PixelOS / Android 15)**  
เวอร์ชันนี้ถูกออกแบบมาให้ “แรงสุดแต่ยังปลอดภัย”  
โดยจะปรับพลัง CPU, GPU, และ System UI แบบอัตโนมัติเมื่อเปิดแอป **Lalamove / Google Maps**

---

## ⚙️ ฟีเจอร์หลัก
- Auto-daemon + Watchdog → ทำงานอัตโนมัติทุกบูต  
- Dynamic CPU/GPU scaling (เร่งเองเมื่อจำเป็น)  
- ปรับ SystemUI scale ให้ลื่นสุด  
- Network & I/O tuning สำหรับแม็พและเน็ตเสถียร  
- Thermal fallback อัตโนมัติเมื่ออุณหภูมิเกิน 50°C  
- รองรับ Magisk, L Speed, FKM (ไม่ชนกัน)

---

## 🔧 ค่าโปรไฟล์พื้นฐาน
| โหมด | CPU Max | Min | หมายเหตุ |
|-------|----------|------|-----------|
| 🚚 Lalamove | 100% | 60% | แรงสุดทุกครั้งเปิดแอป |
| ⚖️ Balanced | 95% | 55% | สมดุลทั่วไป |
| 🌙 Idle | 65% | 45% | ประหยัดพลังงาน |

---

## 📦 การติดตั้ง
1. ดาวน์โหลดไฟล์ ZIP:  
   👉 [Lalamove_Perf_Preset_PocoF3_v2.4_max_release.zip](./Lalamove_Perf_Preset_PocoF3_v2.4_max_release.zip)
2. เปิด **Magisk → Modules → Install from storage**
3. เลือกไฟล์ ZIP → รอจนติดตั้งเสร็จ → รีบูตเครื่อง
4. (ไม่จำเป็น) ปรับค่าใน `/data/local/tmp/lalamove_config.json`

---

## 📊 Logs
- `/data/local/tmp/lalamove_daemon_v2.4.log`  
- `/data/local/tmp/lalamove_unified_runtime_v2.4.log`  
- `/data/local/tmp/lalamove_watchdog_v2.4.log`

---

## 💡 เคล็ดลับ
- แนะนำใช้คู่กับ **FKM / SmartPack / KernelSU**
- ห้ามเปิดแอป L Speed พร้อมกันถ้าไม่ได้ตั้ง “Custom mode”
- ถ้าอยากดูสถานะจริง → ใช้คำสั่ง `logcat | grep lalamove`

---

🧩 **Tuned by ChatGPT Assistant**  
Optimized for **Snapdragon 870 / POCO F3 / PixelOS 15**
