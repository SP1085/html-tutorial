---
layout: default
title: ฟอร์ม HTML
nav_order: 9
---

# ฟอร์ม HTML

## 🔹 ฟอร์มคืออะไร?

**ฟอร์ม (Form)** ใน HTML คือส่วนที่ใช้สำหรับรับข้อมูลจากผู้ใช้ เช่น แบบฟอร์มสมัครสมาชิก, ฟอร์มติดต่อเรา, ช่องค้นหา

ฟอร์มใน HTML เริ่มต้นด้วยแท็ก `<form>` และมีองค์ประกอบภายใน เช่น `<input>`, `<textarea>`, `<select>`, `<button>`

---

## 🔸 โครงสร้างพื้นฐานของฟอร์ม

```html
<form action="/submit" method="post">
  <label>ชื่อ:</label>
  <input type="text" name="name" />
  <br />
  <label>อีเมล:</label>
  <input type="email" name="email" />
  <br />
  <button type="submit">ส่งข้อมูล</button>
</form>
```

### 🔍 อธิบาย:

- `action` คือ URL ที่จะส่งข้อมูลไป
- `method` คือวิธีส่งข้อมูล (GET หรือ POST)

---

## 🔸 ประเภทของ `<input>`

| type        | ใช้สำหรับ             |
|-------------|------------------------|
| `text`      | ข้อความทั่วไป         |
| `email`     | อีเมล                  |
| `password`  | รหัสผ่าน               |
| `number`    | ตัวเลข                 |
| `checkbox`  | ตัวเลือกหลายรายการ    |
| `radio`     | ตัวเลือกเดียวจากกลุ่ม |
| `submit`    | ปุ่มส่งข้อมูล          |

```html
<input type="text" />
<input type="password" />
<input type="checkbox" />
<input type="radio" />
```

---

## 🔸 ช่องข้อความหลายบรรทัด: `<textarea>`

```html
<textarea name="message" rows="4" cols="30">
ข้อความที่ผู้ใช้พิมพ์...
</textarea>
```

---

## 🔸 รายการให้เลือก: `<select>`

```html
<select name="gender">
  <option value="male">ชาย</option>
  <option value="female">หญิง</option>
</select>
```

---

## 🔸 ปุ่มในฟอร์ม

```html
<button type="submit">ส่ง</button>
<button type="reset">ล้าง</button>
```

---

## 🔸 ตัวอย่างฟอร์มที่สมบูรณ์

```html
<form action="/register" method="post">
  <label>ชื่อผู้ใช้:</label>
  <input type="text" name="username" required />
  <br />
  <label>รหัสผ่าน:</label>
  <input type="password" name="password" required />
  <br />
  <label>เพศ:</label>
  <input type="radio" name="gender" value="male" /> ชาย
  <input type="radio" name="gender" value="female" /> หญิง
  <br />
  <label>ความสนใจ:</label>
  <input type="checkbox" name="interest" value="html" /> HTML
  <input type="checkbox" name="interest" value="css" /> CSS
  <br />
  <label>ประเทศ:</label>
  <select name="country">
    <option value="th">ไทย</option>
    <option value="jp">ญี่ปุ่น</option>
  </select>
  <br />
  <label>หมายเหตุ:</label>
  <textarea name="note" rows="4"></textarea>
  <br />
  <button type="submit">สมัครสมาชิก</button>
</form>
```

---

## 🧠 สรุป

- ใช้ `<form>` ครอบทุก input
- ใช้ `action` และ `method` เพื่อกำหนดการส่งข้อมูล
- มีหลายชนิดของ input ให้เลือกใช้งาน
- อย่าลืมใส่ `name` ในทุก input เพื่อส่งข้อมูลให้ server

---

👉 ไปยังบทถัดไป: [สื่อมีเดีย: <audio>, <video>](html-09-media.md)
