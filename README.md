# Bank Greeting - CS50P Problem Set 1

برنامه‌ای که میزان جایزه را بر اساس نوع احوال‌پرسی کاربر تعیین می‌کند.

## 🎯 شرايط برنامه
- اگر کاربر با **"hello"** شروع کند: خروجی `$0`
- اگر با **"h"** (غیر از "hello") شروع شود: خروجی `$20`
- در غیر این صورت: خروجی `$100`


---

### **۳. بهبود کد (`bank.py`) با کامنت‌گذاری**
```python
# دریافت ورودی کاربر و نرمال‌سازی آن (حذف فاصله‌ها + حروف کوچک)
greeting = input("Greeting: ").strip().lower()

# بررسی شرایط جایزه
if greeting.startswith("hello"):
    print("$0")  # حالت hello
elif greeting.startswith("h"):
    print("$20")  # حالت h (غیر از hello)
else:
    print("$100")  # سایر موارد
## 🚀 نحوه اجرا
```bash
python bank.py 
