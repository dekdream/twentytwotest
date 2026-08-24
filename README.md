# HR Management Flutter + Supabase

ระบบ HR starter สำหรับจัดการพนักงาน แผนก ตำแหน่ง ลงเวลา ลางาน เงินเดือน ประกาศ และ Dashboard

## Setup

## Deploy Flutter Web to Railway

Create a Railway service from this GitHub repository. Use the default root directory and start command:

```text
npm start
```

Railway will provide `PORT` automatically. The service serves the Flutter Web files from the repository root.

1. สร้างโปรเจกต์ Supabase แล้วรัน SQL ใน `supabase/schema.sql`
2. ตั้งค่า environment ตอนรันแอป

```powershell
flutter run --dart-define=API_BASE_URL=https://your-api-service.example.com
```

ถ้ายังไม่ใส่ค่า Supabase แอปจะเปิดได้ แต่ข้อมูลจะว่างและ action ที่ต้องเชื่อมต่อฐานข้อมูลจะไม่ทำงาน

## Default Modules

- Login ผ่าน Supabase Auth
- Dashboard สรุปจำนวนพนักงาน การเข้างาน การลา ขาดงาน และประกาศล่าสุด
- Employees, Departments, Positions
- Attendance
- Leave Requests
- Payroll
- Announcements
