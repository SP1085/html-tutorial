---
layout: default
title: Meta tag และ SEO
nav_order: 12
---

# Meta tag และ SEO

## 🔹 Meta tag คืออะไร?

**Meta tag** เป็นแท็ก HTML ที่อยู่ใน `<head>` ของเอกสาร  
ใช้เพื่อเก็บข้อมูลเกี่ยวกับหน้าเว็บ เช่น คำอธิบาย คำสำคัญ ผู้เขียน และการเข้ารหัสอักขระ

Meta tag ไม่แสดงผลบนหน้าเว็บ แต่มีความสำคัญต่อ:
- การแสดงผลในเครื่องมือค้นหา (SEO)
- การแชร์บนโซเชียลมีเดีย
- การตั้งค่าการแสดงผลของเบราว์เซอร์

---

## 🔸 ตัวอย่าง Meta tag ที่ใช้บ่อย

```html
<head>
  <meta charset="UTF-8" />
  <meta name="description" content="บทเรียน HTML สำหรับผู้เริ่มต้น" />
  <meta name="keywords" content="HTML, เริ่มต้น, เว็บไซต์" />
  <meta name="author" content="สรรภัส สังเกตุ" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>บทเรียน HTML</title>
</head>
```

---

## 🔸 คำอธิบาย meta tag

| แท็ก | ความหมาย |
|------|-----------|
| `charset` | กำหนดชุดอักขระ เช่น UTF-8 |
| `description` | คำอธิบายสั้น ๆ ของหน้าเว็บ |
| `keywords` | คำสำคัญที่เกี่ยวข้องกับเนื้อหา |
| `author` | ชื่อผู้เขียน |
| `viewport` | กำหนดการแสดงผลบนอุปกรณ์พกพา |

---

## 🔸 Meta สำหรับ SEO

แม้ว่า Google จะไม่ได้ใช้ `<meta name="keywords">` โดยตรง  
แต่การใส่ `<meta name="description">` จะช่วยในการแสดงข้อความใต้ชื่อเว็บไซต์บน Google

ตัวอย่าง:

```html
<meta name="description" content="เรียนรู้ HTML เบื้องต้น พร้อมตัวอย่างเข้าใจง่าย">
```

> ✅ ควรใช้คำอธิบายที่สั้น กระชับ และสื่อสารชัดเจน

---

## 🔸 Meta สำหรับ Social Media (Open Graph)

สำหรับการแชร์ลิงก์บน Facebook, LINE, Twitter ให้แสดงภาพและชื่ออย่างถูกต้อง

```html
<meta property="og:title" content="สอน HTML ฟรี" />
<meta property="og:description" content="เริ่มต้นเรียน HTML อย่างเข้าใจง่าย" />
<meta property="og:image" content="https://example.com/cover.jpg" />
<meta property="og:url" content="https://example.com/html-tutorial" />
```

---

## ❗ ข้อควรระวัง

- อย่าลืมใส่ `<meta charset="UTF-8">` ไว้บรรทัดแรกใน `<head>` เพื่อป้องกันภาษาไทยเพี้ยน
- คำอธิบาย (`description`) ควรไม่เกิน 150-160 ตัวอักษร
- ตรวจสอบด้วย [Google Rich Results Test](https://search.google.com/test/rich-results)

---

## 🧠 สรุป

- Meta tag สำคัญแม้จะไม่แสดงผล
- ใช้เพื่อบอกข้อมูลเบื้องหลังแก่เบราว์เซอร์และ Search Engine
- ควรใส่ใน `<head>` ทุกหน้า
- ส่งผลโดยตรงต่อ SEO และการแชร์ลิงก์

---

👉 ไปยังบทถัดไป: [แนวทางการเขียน HTML ที่ดี](html-12-best-practices.md)
