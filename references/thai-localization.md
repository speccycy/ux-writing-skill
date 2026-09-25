# Thai Localization for Gaming Web Apps

Localize meaning, state, and action. Do not mirror English sentence structure.

## Principles

### Write Thai as Thai
Prefer natural Thai word order and remove words that only exist because the English source has them.

English:
- Unable to start server.

Avoid:
- ไม่สามารถเริ่มต้นเซิร์ฟเวอร์ได้

Prefer:
- เปิดเซิร์ฟเวอร์ไม่สำเร็จ

### Keep useful technical English
Keep commonly understood technical terms in English when translation would sound less natural or less precise.

Usually keep:
- Server
- Console
- Backup
- Restore
- Mod
- Plugin
- Node
- RCON
- API
- CPU
- RAM
- DDoS
- Discord

Translate the surrounding action naturally.

Examples:
- เปิด Server
- ดู Console
- สร้าง Backup
- Restore จาก Backup
- เชื่อมต่อ Discord

If the product already has an established Thai term, use that consistently instead.

### Avoid overly formal Thai
Avoid routine UI wording such as:
- โปรดดำเนินการ
- ไม่สามารถดำเนินการได้
- การดำเนินการดังกล่าว
- กรุณาทำการ
- เนื่องจากเกิดข้อผิดพลาดที่ไม่คาดคิด

Prefer direct forms:
- ลองอีกครั้ง
- บันทึกไม่สำเร็จ
- เปิด Server ไม่สำเร็จ
- เชื่อมต่อไม่ได้

### Avoid unnecessary pronouns
English often needs "you/your"; Thai often does not.

English:
- Your server is ready.

Natural Thai:
- Server พร้อมใช้งานแล้ว

Not:
- Server ของคุณพร้อมใช้งานแล้ว

Use **ของคุณ** only when ownership needs emphasis or disambiguation.

### Routine UI usually does not need ครับ/ค่ะ
Avoid adding politeness particles to:
- buttons
- labels
- status
- validation
- routine errors
- toasts

Use polite particles only when the product intentionally speaks like human support or in a conversational assistant.

## Button examples

| English | Thai |
|---|---|
| Start server | เปิด Server |
| Stop server | ปิด Server |
| Restart server | Restart Server |
| Create backup | สร้าง Backup |
| Restore backup | Restore Backup |
| Save changes | บันทึก |
| View console | ดู Console |
| Copy IP address | คัดลอก IP |
| Join Discord | เข้า Discord |
| Renew subscription | ต่ออายุ |

Do not force Thai translations for terms users recognize faster in English.

## Status examples

| English | Thai |
|---|---|
| Starting | กำลังเปิด |
| Running | กำลังทำงาน |
| Restarting | กำลัง Restart |
| Stopping | กำลังปิด |
| Updating | กำลังอัปเดต |
| Backing up | กำลัง Backup |
| Restoring | กำลัง Restore |
| Offline | Offline |
| Maintenance | ปิดปรับปรุง |
| Unavailable | ใช้งานไม่ได้ชั่วคราว |

Choose terminology that matches the rest of the product.

## Error examples

English:
- Server failed to start. Check the console for the latest error.

Thai:
- เปิด Server ไม่สำเร็จ ตรวจสอบ error ล่าสุดได้ที่ Console

English:
- Backup failed. There isn't enough storage available.

Thai:
- Backup ไม่สำเร็จ พื้นที่จัดเก็บไม่เพียงพอ

English:
- Connection lost. Reconnect to continue viewing the console.

Thai:
- การเชื่อมต่อหลุด เชื่อมต่อใหม่เพื่อดู Console ต่อ

## Destructive actions

English:
- Wipe server data?
- This removes the current world and player data. Server settings are kept.

Thai:
- ล้างข้อมูล Server?
- ระบบจะลบข้อมูลโลกและผู้เล่นปัจจุบัน แต่ยังเก็บการตั้งค่า Server ไว้

Primary action:
- ล้างข้อมูล Server

Avoid vague buttons such as:
- ยืนยัน
- ตกลง

when the destructive action can be named directly.

## Billing examples

English:
- Payment failed. Update your payment method to keep the server active.

Thai:
- ชำระเงินไม่สำเร็จ อัปเดตวิธีชำระเงินเพื่อให้ Server ใช้งานต่อได้

English:
- Subscription expired.

Thai:
- แพ็กเกจหมดอายุแล้ว

Use **แพ็กเกจ**, **บริการ**, or **Subscription** according to the product's established terminology; do not mix them randomly.

## Translation audit

Before finalizing Thai:
- Does it sound like a Thai product, not a translated manual?
- Can any pronoun be removed?
- Can formal filler be removed?
- Are technical English terms preserved where useful?
- Does the Thai version communicate the same consequence and recovery action as English?
- Is the Thai shorter without losing operational meaning?
