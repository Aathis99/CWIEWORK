- ระบบ login/logout
- ระบบจัดการสินค้า (CRUD)
- ไฟล์ฐานข้อมูลคือ 66162150104_db.sql


# ระบบ จัดการสินค้า: react/nodejs-express/bootstarp

## วิธีติดตั้งและเริ่มใช้งาน

ทำตามขั้นตอนเหล่านี้เพื่อรันส่วนหน้าบ้านในเครื่องของคุณ:

1.  **คัดลอกโปรเจกต์ (Clone repository):**
    เปิด Terminal (หรือ Command Prompt / Git Bash) แล้วพิมพ์คำสั่ง:
    ```bash
    git clone [https://github.com/ช](https://github.com/ช)ื่อผู้ใช้_ของคุณ/ชื่อ_repo_frontend_ของคุณ.git
    cd ชื่อ_repo_frontend_ของคุณ
    ```
    * (เปลี่ยน `ชื่อผู้ใช้_ของคุณ/ชื่อ_repo_frontend_ของคุณ.git` เป็น URL GitHub Repository จริงของคุณ)

2.  **ติดตั้ง Packages ที่จำเป็น:**
    ```bash
    npm install
    ```

3.  **ตั้งค่าตัวแปรสภาพแวดล้อม (.env):**
    สร้างไฟล์ชื่อ `.env` ในโฟลเดอร์หลักของโปรเจกต์ `frontend` ของคุณ (อยู่ในระดับเดียวกับ `package.json`).
    ไฟล์นี้จะเก็บ URL ของ API Backend ของคุณ.
    แทนที่ `URL_BACKEND_API_ของคุณ` ด้วย URL จริงของ Backend Server ที่รันอยู่ (เช่น `http://localhost:5000/api` ถ้า Backend รันในเครื่อง, หรือ URL จาก Render ถ้า Deploy แล้ว).

    ```dotenv
    VITE_API_URL=URL_BACKEND_API_ของคุณ
    ```
    *ตัวอย่าง (รันในเครื่อง):* `VITE_API_URL=http://localhost:5000/api`
    *ตัวอย่าง (ถ้า Deploy แล้ว):* `VITE_API_URL=https://your-backend-api.onrender.com/api`

4.  **รันแอปพลิเคชัน:**
    ```bash
    npm run dev
    ```
    แอปพลิเคชันจะเปิดขึ้นมาใน Browser โดยปกติที่ `http://localhost:5173`
