# Smile Doggy CAFÉ (DOGGY CAFE)

ยินดีต้อนรับสู่โครงการเว็บ "DOGGY CAFE"

---

## โครงสร้างโปรเจค (ไฟล์สำคัญ)
โปรเจคนี้เป็น static site โดยไฟล์สำคัญที่มีใน repository นี้คือ:

```
/project-root
├─ index.html
├─ README.md
├─ css/
│  ├─ animate.css
│  ├─ owl.carousel.min.css
│  ├─ owl.theme.default.min.css
│  ├─ magnific-popup.css
│  ├─ bootstrap-datepicker.css
│  ├─ jquery.timepicker.css
│  ├─ flaticon.css
│  └─ style.css
├─ js/
│  ├─ jquery.min.js
│  ├─ jquery-migrate-3.0.1.min.js
│  ├─ popper.min.js
│  ├─ bootstrap.min.js
│  ├─ jquery.easing.1.3.js
│  ├─ jquery.waypoints.min.js
│  ├─ jquery.stellar.min.js
│  ├─ jquery.animateNumber.min.js
│  ├─ bootstrap-datepicker.js
│  ├─ jquery.timepicker.min.js
│  ├─ owl.carousel.min.js
│  ├─ jquery.magnific-popup.min.js
│  ├─ scrollax.min.js
│  ├─ google-map.js
│  └─ main.js
└─ images/
```

---

## การรันโปรเจค (Local)
1. เปิดไฟล์ index.html โดยตรง (ทดสอบเร็ว) หรือ
2. ใช้ HTTP server (แนะนำ) เช่น Python:
   - python -m http.server 8000
   - เข้า: http://localhost:8000

---

## หมายเหตุการแก้ไขที่ทำในไฟล์ index.html
- แก้ปุ่ม "Add to cart" ที่ปิดด้วยแท็กผิด (</a>) เป็น </button> เพื่อให้ HTML ถูกต้องและปุ่มทำงานได้
- ปรับ path รูปที่มีช่องว่างให้เป็น quoted URL (ตัวอย่าง: 'images/cake/Chocolate Lava Cakes.jpg')
- เพิ่ม overlay element:
  - <div id="offcanvasOverlay" class="offcanvas-overlay" onclick="closeSidebar()"></div>
  เพื่อให้ overlay ด้านหลังทำงานเมื่อเปิด sidebar
- ปรับสคริปต์ openSidebar/closeSidebar ให้เช็คการมีอยู่ของ element ก่อนเรียก classList เพื่อป้องกัน error ถ้า element ยังไม่อยู่ใน DOM

---

## แนะนำการปรับแต่งสั้นๆ
- เพิ่ม/แก้ไขเมนู: แก้ใน index.html ที่บล็อกเมนู (div class="block-7")
- เปลี่ยนสไตล์: แก้ css/style.css
- เชื่อม backend: เปลี่ยนปุ่มหรือฟอร์มเป็นการ POST ไปยัง API ของคุณ

---

หากต้องการ ผมสามารถช่วย:
- สร้างตัวอย่างไฟล์ css/style.css จากรูปแบบที่ต้องการ
- สร้างตัวอย่าง main.js สำหรับจัดการ cart แบบง่าย
บอกได้ว่าต้องการเพิ่มอะไรต่อไปครับ
