## ควบคุม Seven Segment วนลูปแสดงตัวเลข 0-9 โดยสลับทุกๆ 1 วินาที อิงจากแลป Seven Segment
การควบคุมSeven Segment วนลูปแสดงตัวเลข 0-9  เป็นพื้นฐานการเริ่มต้นที่ง่ายในการใช้Seven Segmentจึงเลือกมาเพื่อเป็นการสาธิตในกระบวนการทำที่ไม่ซับซ้อน
1.เปิด VS Code และใช้คำสั่ง Create ESP-IDF Project เพื่อสร้างโปรเจกต์ใหม่ เลือกบอร์ด ESP32 และตั้งชื่อโปรเจกต์

<img width="895" alt="image" src="https://github.com/user-attachments/assets/8b972390-4f20-4b32-aa00-66df6c073b02">

2. เชื่อมต่อ Seven Segment กับ ESP32
Seven Segment Display มี 7 พินที่ต้องเชื่อมต่อกับ GPIO ของ ESP32 เพื่อแสดงผล

ให้เลือก GPIO ที่ต้องการใช้สำหรับ Seven Segment Display (เช่น GPIO 0, GPIO 2, GPIO 4,)
เชื่อมต่อพิน A-G ของ Seven Segment กับ GPIO ที่เลือกไว้
ตั้งค่า PWR หรือ GND ตามที่จำเป็น
 
 3.เขียนโค้ดสำหรับควบคุมวนลูปแสดงตัวเลข 0-9 โดยสลับทุกๆ 1 วินาที
 
 ![Screenshot 2024-11-09 020008](https://github.com/user-attachments/assets/8956b840-4dd3-463e-b8fa-259680afa3f9)

 ![Screenshot 2024-11-09 020025](https://github.com/user-attachments/assets/40d38f63-ec41-476e-a41b-e80144cd3e7c)

 ![Screenshot 2024-11-09 020041](https://github.com/user-attachments/assets/d0a653c6-663a-4abf-8f07-975bc966df0a)

4.คอมไพล์และอัปโหลดโค้ดไปยัง ESP32
Build, Flash and Monitor เพื่อคอมไพล์และอัปโหลดโค้ดไปยัง ESP32
ถ้าเชื่อมต่อบอร์ดสำเร็จ จะเห็นข้อความใน Serial Monitor และ Seven Segment วนลูปแสดงตัวเลข 0-9


