# 🔐 Random Password Generator  
# 🔐 تولید رمز عبور به‌صورت تصادفی و امن

A simple Python script that generates a secure password based on user-defined length.  
یک اسکریپت ساده پایتون که بر اساس طول دلخواه کاربر، یک رمز عبور امن تولید می‌کند.

---

## 📌 How It Works  
## 📌 این برنامه چگونه کار می‌کند

For each character position (`i`) in the password, the script determines the character type using the remainder of division (`%`) as follows:  
برای هر موقعیت (یا اندیس `i`) در رمز عبور، نوع کاراکتر با استفاده از باقیمانده تقسیم (`%`) به شکل زیر مشخص می‌شود:

| Condition (i % x) | Character Type     |  
|------------------|--------------------|  
| i % 4 == 0       | Uppercase letter   |  
| i % 3 == 0       | Symbol             |  
| i % 2 == 0       | Lowercase letter   |  
| Else             | Digit              |  

| شرط تقسیم اندیس     | نوع کاراکتر انتخابی       |  
|----------------------|---------------------------|  
| i بخش‌پذیر بر ۴       | حرف بزرگ انگلیسی         |  
| i بخش‌پذیر بر ۳       | نماد (Symbol)             |  
| i بخش‌پذیر بر ۲       | حرف کوچک انگلیسی         |  
| سایر موارد            | عدد (Digit)               |  

---

## ▶️ How to Run  
## ▶️ نحوه اجرا

1. Make sure **Python 3** is installed.  
   مطمئن شوید که **پایتون نسخه ۳** روی سیستم شما نصب شده باشد.

2. Run the script using the command below:  
   اسکریپت را با دستور زیر اجرا کنید:

```bash
python password_generator.py

3. Enter the desired password length when prompted.
هنگام اجرای برنامه، طول رمز دلخواه را وارد کنید.


💡 Example Output

💡 نمونه خروجی

Enter desired password length: 10  
Generated password: A9d!G7k@P0

طول رمز عبور مورد نظر شما چقدر است؟ ۱۰  
رمز عبور تولید شده برای شما: A9d!G7k@P0

> The output is different each time, based on the index-based logic.
خروجی هر بار اجرا متفاوت است چون وابسته به اندیس‌ها است
