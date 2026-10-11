# Universal POS - MySQL Edition
For Restaurants, Supermarkets, Salons & Bookshops | Kenya | KES | M-Pesa

GitHub: https://github.com/tymesdevan-del/universal_pos.git

## Business Modes (One System)
- SUPERMARKET: Barcode scan, expiry, weight
- RESTAURANT: Tables T1-T20, KDS, Dine-In/Takeaway/Delivery, Split Bill
- SALON: Services, Staff Commission, Appointments
- BOOKSHOP: ISBN, Author, Variants

## Features
Dashboard, POS Checkout (CASH, M-PESA TILL, M-PESA PAYBILL, CARD, CREDIT), Inventory CRUD, Tables, Appointments, Customers, Reports PDF/Excel, 80mm Thermal Receipt, Shifts, Users.

## Tech
React + TypeScript + Tailwind + shadcn + Prisma MySQL

## Setup with MySQL

1. Create database:
CREATE DATABASE universal_pos;

2. Clone:
git clone https://github.com/tymesdevan-del/universal_pos.git
cd universal_pos
npm install

3. Env:
cp .env.example .env
Edit DATABASE_URL to your MySQL: mysql://root:@localhost:3306/universal_pos

4. Push DB:
npx prisma db push

5. Run:
npm run dev

Open http://localhost:3000
Login: admin@pos.com / admin123

## Lovable Deploy
1. Import GitHub repo in lovable.dev
2. Prompt: Build full POS UI on MySQL schema
3. Set DATABASE_URL in Lovable > Settings > Env if using PlanetScale/Railway MySQL
4. Push back to GitHub
