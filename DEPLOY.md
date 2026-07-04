# Deploy EZPOK168 Bio Analytics

โปรเจกต์นี้เป็นหน้า Bio + popup โปรโมชั่น + dashboard สถิติคลิก สำหรับแบรนด์ EZPOK168

## Local

```bash
npm start
```

เปิด:

- `http://localhost:8787/`
- `http://localhost:8787/dashboard.html`

ค่า login local เริ่มต้น:

- user: `admin`
- password: `ezpok1682026`

## Render Blueprint

1. อัปโหลดโฟลเดอร์นี้ขึ้น GitHub
2. เข้า Render > New > Blueprint
3. เลือก repo ที่อัปโหลดไว้
4. Render จะอ่าน `render.yaml`
5. ตั้ง `DASHBOARD_PASSWORD`
6. Deploy

หลัง deploy:

- หน้า Bio: `https://ชื่อ-service.onrender.com/`
- Dashboard: `https://ชื่อ-service.onrender.com/dashboard.html`

## หมายเหตุ

- ระบบสถิติเก็บใน persistent disk ที่ `/var/data`
- อย่าเปิดเว็บด้วย `file:///...` เมื่อต้องการเก็บสถิติจริง ให้เปิดผ่าน server URL เท่านั้น
