---
layout: default
title: โครงสร้าง HTML เบื้องต้น
nav_order: 3
---

# โครงสร้าง HTML เบื้องต้น

## 🔹 ส่วนประกอบของ HTML

ทุกหน้าเว็บ HTML จะมีโครงสร้างพื้นฐานเหมือนกัน ซึ่งประกอบด้วย:

- `<!DOCTYPE html>` : ประกาศว่าใช้ HTML เวอร์ชัน 5
- `<html>` : ครอบทุกส่วนของ HTML ทั้งหมด
- `<head>` : เก็บข้อมูลเบื้องหลัง เช่น ชื่อหน้าเว็บ, meta tag, ลิงก์ CSS
- `<body>` : เนื้อหาหลักของเว็บ เช่น ข้อความ, รูปภาพ, ปุ่ม

---

## 🔸 ตัวอย่างโครงสร้าง HTML ที่ถูกต้อง

```html
<!DOCTYPE html>
<html lang="th">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>หน้าแรก</title>
  </head>
  <body>
    <h1>ยินดีต้อนรับสู่เว็บไซต์ของฉัน</h1>
    <p>นี่คือเว็บไซต์ตัวอย่างที่ใช้ HTML พื้นฐาน</p>
  </body>
</html>
```

---

## 🔸 คำอธิบายโครงสร้าง

| แท็ก | ความหมาย |
|------|-----------|
| `<!DOCTYPE html>` | ระบุว่าใช้ HTML5 |
| `<html>` | แท็กหลักที่ครอบเนื้อหาทั้งหมด |
| `<head>` | ส่วนหัว ใช้กำหนดข้อมูลพื้นฐาน |
| `<title>` | ชื่อแท็บที่ปรากฏบนเบราว์เซอร์ |
| `<meta charset="UTF-8">` | กำหนดรหัสอักขระให้รองรับภาษาไทย |
| `<body>` | ส่วนแสดงเนื้อหาหลัก |

---

## 🔸 โครงสร้างพื้นฐาน (Minimal HTML)

```html
<!DOCTYPE html>
<html>
  <head>
    <title>เว็บของฉัน</title>
  </head>
  <body>
    <p>สวัสดี HTML!</p>
  </body>
</html>
```

---

## 🧠 สรุป

- HTML ทุกหน้าเริ่มด้วย `<!DOCTYPE html>`
- มี 2 ส่วนหลักคือ `<head>` และ `<body>`
- จัดโครงสร้างอย่างเป็นระเบียบเพื่อให้อ่านง่าย
- การใส่ `meta charset="UTF-8"` สำคัญสำหรับภาษาไทย

---

👉 ไปยังบทถัดไป: [แท็กข้อความ: <h1> - <p>, <br>](html-03-tags-text.md)
