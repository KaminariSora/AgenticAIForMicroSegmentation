# Run Project
1. install requirements

    `pip install -r requirements.txt`
---
2. ไปเอา API KEY จาก google_api มาก่อนจากเว็บ 

    `https://aistudio.google.com/app/api-keys`
---
3. สร้างไฟล์ `.env` ใน Directory `./agenticAIforMicrosegmentation` จากนั้นเขียนตามนี้ในไฟล์ `.env`

    `GOOGLE_API_KEY=[ใส่ Key]`
---
4. รันโปรแกรมหลัก

    `python main.py`


# Error Case
1. `Value error, API key required for Gemini Developer API`

    1.1 ลองไปเช็ค Path ของ `.env`

    1.2 เช็ค Path ของ `model_cofig.py` ตรงบรรทัดที่ 7

    `env_path = Path([ใส่ Path ของ .env ให้ถูก])`