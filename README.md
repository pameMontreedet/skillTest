# skillTest
1. Install dotnet v2.1.3 (ถ้าเครื่องยังไม่ได้ลง)
2. Cd ไปที่ Path ProjectSkillTest
3. รันคำสั่ง docker-compose up -d
4. Cd ไปที่ Path Applib
5. รันไฟล์ db-update.sh
6. เช็ดที่ SQL Server จะมี Table ขึ้นมา
7. Cd ไปที่ Path AppBackend
8. รันไฟล์ dotnet-run.sh

เช็ค Api แต่ละเส้นครับ (ตามชื่อ Action ใน Controller ครับ)

Api การสมัคร : https://localhost:5001/api/Card/RegisterCard

Api การเติมรอบ : https://localhost:5001/api/Card/AddRound/{IDของบัตร}

Api การเติมเงิน : https://localhost:5001/api/Card/AddMoney/{IDของบัตร}

Api การหักตอนประตูขาออก : https://localhost:5001/api/Card/Deduction/{IDของบัตร}

Cd ไปที่ Path Apptest (สำหรับ Test)

รันคำสั่ง. dotnet test
