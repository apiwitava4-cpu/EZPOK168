# Next Steps: GitHub + Render

สถานะที่ควรทำต่อหลังตรวจ local ผ่าน:

1. สร้าง GitHub repo ใหม่ เช่น `ezpok168-bio`
2. push โฟลเดอร์นี้ขึ้น branch `main`
3. เข้า Render > New > Blueprint
4. เลือก GitHub repo
5. ตั้ง `DASHBOARD_PASSWORD`
6. กด Deploy

ค่าใน `render.yaml`:

- service: `ezpok168-bio-analytics`
- disk: `ezpok168-bio-data`
- region: `singapore`
- data path: `/var/data`
