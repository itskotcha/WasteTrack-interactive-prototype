# WasteTrack prototype

โปรเจกต์เป็น static site (ไม่ต้อง build) โฟลเดอร์ที่เผยแพร่คือ `dist/`

## วิธีที่ 1: Vercel CLI
    npm i -g vercel      # ครั้งแรกครั้งเดียว
    vercel login
    vercel --prod        # ตอบ Enter ตามค่าเริ่มต้นได้เลย (อ่านค่าจาก vercel.json)

## วิธีที่ 2: ผ่าน GitHub
1. push โฟลเดอร์นี้ขึ้น GitHub
2. vercel.com → Add New → Project → เลือก repo
3. Framework Preset = Other, ไม่ต้องใส่ Build Command (vercel.json ตั้งค่า Output Directory = dist ให้แล้ว) → Deploy

## ทดสอบในเครื่อง
    npx serve dist
