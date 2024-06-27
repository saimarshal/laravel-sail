# laravel-sail

* ติดตั้งตามเว็บไซต์
```sh
https://samrid.com/laravel-docker-setting-up/
```

# ใช้คำสั่ง sail แทน ./vendor/bin/sail

1. เปิดไฟล์คอนฟิก shell:
* หากคุณใช้ Bash ให้เปิดไฟล์ ~/.bashrc หรือ ~/.bash_profile
```sh
vi ~/.bashrc
```
หรือ
```sh
vi ~/.bash_profile
```

2. เพิ่ม alias สำหรับ sail:
* เพิ่มบรรทัดนี้ลงในไฟล์
```sh
alias sail='[ -f sail ] && bash sail || bash vendor/bin/sail'
```
3. บันทึกและปิดไฟล์:
* บันทึกการเปลี่ยนแปลงและปิดไฟล์

4. โหลดการตั้งค่าใหม่:
* ใช้คำสั่งต่อไปนี้เพื่อโหลดการตั้งค่าใหม่โดยไม่ต้องรีสตาร์ท terminal
```sh
source ~/.bashrc
```
หรือ
```sh
source ~/.bash_profile
```

ทดสอบคำสั่ง sail
```sh
sail up -d
sail artisan migrate
```

# หากไม่สามารถเชื่อมต่อฐานข้อมูลได้
```sh
sail artisan migrate
```


