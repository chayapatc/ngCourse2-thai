# ไดเร็กทีฟ (Directives)

ไดเร็กทีฟเป็นเอนทิตีที่ใช้ในการเปลี่ยนคุณลักษณะของคอมโพเนนท์หรือเอเลเมนท์และเป็นหนึ่งในหัวใจของ Angular 2 ที่ใช้ในการพัฒนาแอปพลิเคชัน ในความจริงแล้วคอมโพเนนท์ของ Angular 2 เป็นส่วนหนึ่งของไดเร็กทีฟที่มีเทมเพลตเป็นเหตุผลว่าทำไมคอมโพเนนท์จึงถูกส่งเป็น children ผ่านพร็อปเพอร์ตี้ของไดเร็กทีฟ

คอมโพเนนท์ของ Angular 2 ได้ทำหน้าที่แทนไดเร็กทีฟของ Angular 1 ในหลายส่วนที่เคยทำ ปัญหาหลักในจัดการกับเทมเพลตและ dependency injection จะถูกจัดการโดยคอมโพเนนท์ส่วนปัญหาในการแก้ไขคุณลักษณะทั่วไปจะจัดการโดยไดเร็กทีฟ

ใน Angular 2 มีไดเร็กทีฟหลัก ๆ อยู่ 2 ประเภท:
* _ไดเร็กทีฟแบบแอดทริบิวต์ (Attribute directives)_ - ไดเร็กทีฟทีแก้ไขคุณลักษณะของคอมโพเนนท์หรือเอเลเมนท์โดยที่ไม่ยุ่งเกี่ยวกับเทมเพลต
* _ไดเร็กทีฟแบบโครงสร้าง (Structural directives)_ - ไดเร็กทีฟที่แก้ไขคุณลักษณะของคอมโพเนนท์หรือเอเลเมนท์โดยยุ่งเกี่ยวกับวิธีการแสดงผลของเทมเพลต