---
layout: default
title: ตาราง HTML
nav_order: 8
---

# ตาราง HTML

## 🔹 ตารางคืออะไร?

**ตาราง (Table)** ใช้แสดงข้อมูลที่จัดเป็นแถวและคอลัมน์ เช่น ตารางรายชื่อ, ราคาสินค้า, ตารางเวลา ฯลฯ  
HTML ใช้แท็ก `<table>` ร่วมกับ `<tr>`, `<th>`, และ `<td>` เพื่อสร้างตาราง

---

## 🔸 โครงสร้างตารางพื้นฐาน

```html
<table>
  <tr>
    <th>ชื่อ</th>
    <th>อายุ</th>
  </tr>
  <tr>
    <td>สมชาย</td>
    <td>25</td>
  </tr>
  <tr>
    <td>สมหญิง</td>
    <td>30</td>
  </tr>
</table>
```

### อธิบายแท็ก:

| แท็ก | ความหมาย |
|------|-----------|
| `<table>` | แท็กหลักของตาราง |
| `<tr>` (table row) | แถวของตาราง |
| `<th>` (table header) | หัวคอลัมน์ (ตัวหนา กึ่งกลาง) |
| `<td>` (table data) | ข้อมูลในแต่ละช่อง |

---

## 🔸 กำหนดเส้นขอบ (border)

```html
<table border="1">
  <tr>
    <th>สินค้า</th>
    <th>ราคา</th>
  </tr>
  <tr>
    <td>ข้าว</td>
    <td>30</td>
  </tr>
</table>
```

> 📌 ปัจจุบันนิยมกำหนดขอบตารางด้วย CSS เช่น `border: 1px solid black;`

---

## 🔸 รวมเซลล์ (colspan และ rowspan)

### รวมคอลัมน์ (แนวนอน):

```html
<tr>
  <td colspan="2">รวม 2 คอลัมน์</td>
</tr>
```

### รวมแถว (แนวตั้ง):

```html
<tr>
  <td rowspan="2">รวม 2 แถว</td>
  <td>แถวที่ 1</td>
</tr>
<tr>
  <td>แถวที่ 2</td>
</tr>
```

---

## 🔸 ใช้ร่วมกับ CSS (ตัวอย่าง)

```html
<table style="border-collapse: collapse; width: 100%;">
  <tr>
    <th style="border: 1px solid #000;">หัวข้อ</th>
    <th style="border: 1px solid #000;">ข้อมูล</th>
  </tr>
  <tr>
    <td style="border: 1px solid #000;">ตัวอย่าง</td>
    <td style="border: 1px solid #000;">12345</td>
  </tr>
</table>
```

---

## 🧠 สรุป

| แท็ก | ใช้ทำอะไร |
|------|------------|
| `<table>` | สร้างตาราง |
| `<tr>` | แถวของตาราง |
| `<th>` | หัวคอลัมน์ |
| `<td>` | ข้อมูลทั่วไป |
| `colspan` / `rowspan` | รวมช่องตารางแนวนอน/แนวตั้ง |

- ใช้ CSS เพื่อปรับขอบและความสวยงาม
- หลีกเลี่ยงการใช้ `<table>` เพื่อจัด Layout

---

👉 ไปยังบทถัดไป: [ฟอร์ม HTML](html-08-forms.md)
