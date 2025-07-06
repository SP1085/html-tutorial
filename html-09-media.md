---
layout: default
title: สื่อมีเดีย
nav_order: 10
---

# สื่อมีเดีย: `<audio>`, `<video>`

## 🔹 HTML รองรับสื่อมีเดียอะไรบ้าง?

HTML5 รองรับการแสดง **เสียง (Audio)** และ **วิดีโอ (Video)** โดยตรงผ่านแท็กเฉพาะ  
ทำให้ผู้ใช้สามารถดูหรือฟังได้โดยไม่ต้องใช้ปลั๊กอินภายนอก เช่น Flash

---

## 🔸 การแสดงเสียงด้วย `<audio>`

```html
<audio controls>
  <source src="sound.mp3" type="audio/mpeg" />
  เบราว์เซอร์ของคุณไม่รองรับการเล่นเสียง
</audio>
```

### 🔍 อธิบาย:

- `controls` : แสดงปุ่มเล่น/หยุด/เลื่อน
- `<source>` : ระบุไฟล์เสียงและชนิดไฟล์
- ข้อความระหว่าง `<audio>` ใช้แสดงหากไม่รองรับ

### 🔊 รองรับไฟล์เสียงประเภท:

- `.mp3`
- `.ogg`
- `.wav`

---

## 🔸 การแสดงวิดีโอด้วย `<video>`

```html
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4" />
  เบราว์เซอร์ของคุณไม่รองรับการเล่นวิดีโอ
</video>
```

### 🔍 อธิบาย:

- `width` และ `height` : ขนาดของวิดีโอ
- `controls` : แสดงปุ่มควบคุมวิดีโอ
- `<source>` : ระบุไฟล์วิดีโอและชนิดไฟล์

### 📽️ รองรับไฟล์วิดีโอประเภท:

- `.mp4` (`video/mp4`)
- `.webm` (`video/webm`)
- `.ogg` (`video/ogg`)

<audio controls>
  <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
  ไม่สามารถเล่นเสียง
</audio>

---

## 🔸 คุณสมบัติเสริมของ `<video>`

| คุณสมบัติ | ใช้กับ | ความหมาย |
|------------|--------|-----------|
| `autoplay` | `<audio>`, `<video>` | เล่นอัตโนมัติเมื่อโหลดเสร็จ |
| `loop` | `<audio>`, `<video>` | เล่นวนซ้ำ |
| `muted` | `<video>` | ปิดเสียงเริ่มต้น |
| `poster` | `<video>` | แสดงภาพหน้าปกก่อนเล่น |

```html
<video width="320" height="240" controls autoplay loop muted poster="preview.jpg">
  <source src="video.mp4" type="video/mp4" />
</video>
```

---

## 🧪 ตัวอย่างการแสดงผลวิดีโอจริง

> 🎬 ด้านล่างนี้คือตัวอย่างการแสดงวิดีโอแบบ HTML5  
> (คุณต้องอัปโหลด `video.mp4` และ `preview.jpg` ไว้ในโฟลเดอร์เดียวกัน)

<video width="320" height="240" controls autoplay loop muted poster="preview.jpg">
  <source src="video.mp4" type="video/mp4" />
  เบราว์เซอร์ของคุณไม่รองรับการเล่นวิดีโอ
</video>

<video controls width="300">
  <source src="https://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4">
  ไม่สามารถเล่นวิดีโอ
</video>

---

## ❗ ข้อควรระวัง

- ตรวจสอบว่าไฟล์มีเดียอยู่ใน path ที่ถูกต้อง
- ใช้หลาย `<source>` เพื่อรองรับหลายเบราว์เซอร์
- ไฟล์วิดีโอควรบีบอัดให้เล็กเพื่อโหลดเร็ว

---

## 🧠 สรุป

| แท็ก | ใช้ทำอะไร |
|------|-----------|
| `<audio>` | เล่นไฟล์เสียง |
| `<video>` | เล่นไฟล์วิดีโอ |
| `<source>` | ระบุแหล่งที่มาของไฟล์ |

- ใส่ `controls` เพื่อให้ผู้ใช้ควบคุม
- รองรับไฟล์หลายประเภทเพื่อความเข้ากันได้

---

👉 ไปยังบทถัดไป: [แท็กเชิงโครงสร้าง](html-10-semantics.md)
