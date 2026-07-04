# นักลงทุนน้อย 🌱

เว็บอินเทอร์แอคทีฟสอนลูกเรื่องหุ้นแบบสนุกๆ (ไฟล์เดียว ไม่ต้องมี backend)

## วิธีอัพขึ้น GitHub

```bash
cd little-investor
git init
git add .
git commit -m "first commit: นักลงทุนน้อย"
git branch -M main
git remote add origin https://github.com/<username>/<repo-name>.git
git push -u origin main
```

## วิธี deploy บน Railway

1. ไปที่ https://railway.app → New Project → **Deploy from GitHub repo**
2. เลือก repo ที่ push ไปแล้ว
3. Railway จะเห็น `package.json` แล้วรัน `npm install` + `npm start` ให้อัตโนมัติ (ใช้ Nixpacks)
4. ไปที่ Settings → Networking → กด **Generate Domain** จะได้ลิงก์ เช่น `little-investor.up.railway.app`
5. เปิดลิงก์นั้นได้เลย

ไม่ต้องตั้งค่า Environment Variable ใดๆ เพิ่ม เพราะ Railway จะกำหนด `$PORT` ให้เองอยู่แล้ว
