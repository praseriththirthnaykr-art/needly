# Needly 💜 — Mini Project IS401101

Responsive Web Application ต้นแบบแพลตฟอร์มแบ่งปันความต้องการและความช่วยเหลือในชุมชน ใช้ได้ทั้งมือถือและ PC โดยไม่ต้องใช้ Replit หรือ Backend

## วิธีเปิดในเครื่อง
ดับเบิลคลิกไฟล์ `index.html` เพื่อทดลอง หรือเปิดด้วย Live Server ใน VS Code

## วิธีเผยแพร่ด้วย GitHub Pages (ฟรีสำหรับ Public repository)
1. ลงชื่อเข้าใช้ที่ https://github.com แล้วเลือก **New repository**
2. ตั้งชื่อ Repository เป็น `needly` เลือก **Public** จากนั้นกด **Create repository**
3. เลือก **Add file > Upload files** แล้วอัปโหลดไฟล์ทั้งหมดในโฟลเดอร์นี้ **ไม่ใช่อัปโหลด ZIP โดยตรง** โดย `index.html` ต้องอยู่ที่ root ของ repository
4. กด **Commit changes** (ข้อความปุ่มอาจเปลี่ยนไปตาม UI)
5. เปิด **Settings > Pages** เลือก **Deploy from a branch**; Branch = `main`; Folder = `/(root)` แล้วกด **Save**
6. เมื่อ GitHub Pages เผยแพร่เสร็จ จะได้ลิงก์รูปแบบ `https://USERNAME.github.io/needly/` (เปลี่ยน USERNAME เป็นชื่อ GitHub ของตนเอง)

## คุณสมบัติที่ทำงานได้
- หน้าแรก: ข้อมูลภาพรวม หมวดหมู่ และโพสต์ล่าสุด
- ค้นหาโพสต์: คำค้น หมวดหมู่ สถานะ และลำดับ
- รายละเอียดโพสต์ และปุ่มกดสนใจช่วยแบบเดโม (ไม่ได้ส่งถึงเจ้าของโพสต์จริง)
- Login แบบทดลอง: กรอกชื่อเล่นเท่านั้น ไม่ใช่ระบบยืนยันตัวตนจริง
- สร้างและแก้ไขโพสต์ ตรวจสอบฟอร์ม และจัดการโพสต์ของฉัน
- เปลี่ยนสถานะและลบโพสต์ (มี Confirm)
- Dashboard วิเคราะห์ข้อมูลพร้อมกราฟแท่ง โดนัท และเส้น
- ข้อมูลตัวอย่าง 25 ระเบียน 8 หมวดหมู่ พร้อมปุ่มรีเซ็ตข้อมูล

## หมายเหตุเรื่องความปลอดภัยและข้อมูล
เว็บไซต์เวอร์ชันนี้ใช้ `localStorage` ในแต่ละเบราว์เซอร์ **ไม่ใช่ฐานข้อมูลออนไลน์ที่แชร์กัน** การอัปโหลดไป GitHub ไม่ทำให้ผู้ใช้งานต่างเครื่องเห็นโพสต์ใหม่ร่วมกัน ข้อมูลจำลอง 25 รายการไม่ใช่คำร้องขอจริง บัญชีเป็นเพียงโหมดทดลองซึ่งไม่มีระบบเข้ารหัสหรือยืนยันตัวตน ไม่ควรกรอกข้อมูลส่วนบุคคล รหัสผ่าน หรือ API keys หากต้องใช้งานกับผู้ใช้จริงควรเพิ่มระบบ backend, authentication, database และ moderation

## ข้อกำหนดจากโจทย์
- Input / Process / Output: ครบในการเพิ่ม ค้นหา กรอง และแสดงผล
- 7 หน้าหลัก: Home, Explore, Detail, Create, My Posts, Dashboard, Login (หน้า Edit ใช้โครงสร้างฟอร์ม Create)
- ข้อมูล 25 ระเบียน ฟิลด์ `id`, `title`, `category`, `description`, `location`, `date`, `status`, `owner`, `author`, `helps`
- สถิติ: ผลรวม, ค่าเฉลี่ย, ร้อยละ; กราฟ: bar, doughnut, line; ข้อค้นพบ: 2+ ข้อใน Dashboard
- กรณีทดสอบและ Flowchart อยู่ใน `MINI_PROJECT_NOTES.md`
- ยังต้องจัดทำรายงาน 6–8 หน้า สไลด์ไม่เกิน 8 หน้า และ AI Development Log 3 รายการส่งอาจารย์เพิ่มต่างหาก

## Files
- `index.html` โครงหน้าเว็บ
- `styles.css` หน้าตาและ Responsive
- `data.js` ตัวอย่าง 25 โพสต์
- `app.js` ฟังก์ชันและ Dashboard
- `favicon.svg` ไอคอนเว็บ
- `MINI_PROJECT_NOTES.md` ภาพรวม Flowchart โครงสร้างข้อมูล และชุดทดสอบ
