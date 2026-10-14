# دیتاست نظرات سامسونگ Galaxy A57 در دیجی‌کالا

![License](https://img.shields.io/badge/license-CC--BY--4.0-blue)
![Samples](https://img.shields.io/badge/samples-111-green)
![Language](https://img.shields.io/badge/language-Persian-orange)

یک دیتاست فارسی از نظرات خریداران گوشی **سامسونگ Galaxy A57**، جمع‌آوری‌شده از 
[دیجی‌کالا](https://www.digikala.com/) — بزرگ‌ترین فروشگاه اینترنتی ایران.

این دیتاست برای وظایف **تحلیل احساسات** و **دسته‌بندی متن** به زبان فارسی طراحی شده است.

---

## 📊 خلاصه دیتاست

| ویژگی | مقدار |
|---|---|
| تعداد نمونه | ۱۱۱ |
| زبان | فارسی |
| برچسب‌ها | مثبت، منفی، خنثی |
| منبع | دیجی‌کالا |
| محصول | سامسونگ Galaxy A57 (۲۵۶ گیگابایت، ۸ گیگابایت رم) |
| وظیفه | تحلیل احساسات |
| لایسنس | CC-BY-4.0 |
| بازه‌ی جمع‌آوری | ۱۴۰۵/۰۴/۰۲ تا ۱۴۰۵/۰۷/۲۲ |

---

## 📈 توزیع برچسب‌ها

| برچسب | تعداد | درصد |
|---|---|---|
| positive (مثبت) | ۶۶ | ۵۹.۵٪ |
| negative (منفی) | ۲۹ | ۲۶.۱٪ |
| neutral (خنثی) | ۱۶ | ۱۴.۴٪ |
| **مجموع** | **۱۱۱** | **۱۰۰٪** |

---

## ✅ وضعیت خرید تأییدشده

| وضعیت | تعداد |
|---|---|
| تأییدشده (TRUE) | ۹۲ |
| تأییدنشده (FALSE) | ۱۹ |

---

## 📂 ساختار پروژه
samsung-a57-digikala-reviews/
│
├── README.md # نسخه انگلیسی
├── README_FA.md # این فایل (نسخه فارسی)
├── DATASHEET.md # مستندات کامل (انگلیسی)
├── DATASHEET_FA.md # مستندات کامل (فارسی)
├── LICENSE # لایسنس CC-BY-4.0
│
└── data/
├── clean_comments.csv # دیتاست نهایی (تمیز شده)
└── raw_comments.xlsx # داده‌ی خام

text

---

## 📋 فرمت داده

فایل `clean_comments.csv` این ستون‌ها رو داره:

| ستون | نوع | توضیح |
|---|---|---|
| `id` | عدد | شناسه یکتا |
| `text` | متن | متن نظر (فارسی) |
| `label` | متن | `positive`، `negative`، یا `neutral` |
| `date` | متن | تاریخ نظر (تقویم شمسی) |
| `verified` | بولی | `TRUE` اگر خرید تأییدشده |

### مثال

```csv
id,text,label,date,verified
1,"گوشی خیلی خوبیه، دوربینش عالیه",positive,1405/05/12,TRUE
2,"باتریش زود تموم می‌شه، پشیمون شدم",negative,1405/05/13,TRUE
3,"با A56 فرقش چیه؟",neutral,1405/05/14,FALSE
🚀 نحوه استفاده
python
import pandas as pd

df = pd.read_csv('data/clean_comments.csv', encoding='utf-8-sig')

print(df.head())
print(df['label'].value_counts())
print(f"تعداد کل نمونه‌ها: {len(df)}")
📖 مستندات
برای اطلاعات کامل درباره‌ی انگیزه، ترکیب، فرایند جمع‌آوری، پیش‌پردازش،
کاربردها، توزیع، و محدودیت‌ها:

مستندات انگلیسی

مستندات فارسی

⚠️ محدودیت‌ها
این دیتاست فقط نظرات یک محصول خاص (Galaxy A57) را پوشش می‌دهد.

ممکن است برخی نظرات فیک یا تبلیغاتی باشند.

برچسب‌گذاری توسط یک نفر انجام شده و ممکن است ذهنی باشد.

توزیع کلاس‌ها نامتوازن است (۵۹.۵٪ مثبت).

بعضی نظرات شامل شکایت از قیمت یا لجستیک هستند، نه از خود محصول.

📜 لایسنس
این دیتاست تحت لایسنس
Creative Commons Attribution 4.0 International (CC BY 4.0)
منتشر شده است.

📝 استناد
زرین، ک. (۱۴۰۵). دیتاست نظرات سامسونگ Galaxy A57 در دیجی‌کالا.
GitHub. https://github.com/KosarZarean/samsung-a57-digikala-reviews

📧 تماس
سازنده: کوثر زرین
ایمیل: kzaran79@gmail.com
گیت‌هاب: @KosarZarean

text

---

## قدم‌های آپلود

### ۱. آپلود `README_FA.md`

1. برو تو [repo](https://github.com/KosarZarean/samsung-a57-digikala-reviews)
2. **Add file → Create new file**
3. اسم: `README_FA.md`
4. متن بالا رو پیست کن
5. **Commit new file**

### ۲. آپلود `DATASHEET_FA.md`

1. **Add file → Create new file**
2. اسم: `DATASHEET_FA.md`
3. متن فارسی datasheet (که قبلاً دادم) رو پیست کن
4. **Commit new file**

### ۳. اضافه کردن لینک به `README.md` انگلیسی

برو تو `README.md`، بخش `Documentation` رو اینطور کن:

```markdown
## 📖 Documentation

- [Datasheet (English)](DATASHEET.md)
- [Datasheet (Persian)](DATASHEET_FA.md)
- [README (Persian)](README_FA.md)
ساختار نهایی repo
text
samsung-a57-digikala-reviews/
├── README.md              ← انگلیسی
├── README_FA.md           ← فارسی
├── DATASHEET.md           ← انگلیسی
├── DATASHEET_FA.md        ← فارسی
├── LICENSE
└── data/
    ├── clean_comments.csv
    └── raw_comments.xlsx
