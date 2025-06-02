#import smtplib
from email.mime.multipart import MIMEMultipart
from email.mime.text import MIMEText

# إعدادات البريد
المرسل = "your_email@gmail.com"
كلمة_المرور = "your_app_password"  # استخدم كلمة مرور التطبيق
المستقبل = "aqlan1988@gmail.com"

# إنشاء رسالة
رسالة = MIMEMultipart()
رسالة['From'] = المرسل
رسالة['To'] = المستقبل
رسالة['Subject'] = "حزمة مشروع قرآن الأرض"

# محتوى HTML للبريد
محتوى_بريد = """
[لصق محتوى الحزمة هنا بتنسيق HTML]
"""

# إرفاق المحتوى
رسالة.attach(MIMEText(محتوى_بريد, "html"))

# الإرسال
with smtplib.SMTP_SSL('smtp.gmail.com', 465) as خادم:
    خادم.login(المرسل, كلمة_المرور)
    خادم.sendmail(المرسل, المستقبل, رسالة.as_string()) Aqlan![file_000000006c50623098c261e4d157aa6d](https://github.com/user-attachments/assets/0502453a-410c-49ca-b8be-58b74b36bf65)
![file_000000006c50623098c261e4d157aa6d](https://github.com/user-attachments/assets/15e3b321-d194-47ec-b8ee-0b1616b52014)

https://github.com/Aqlan1988/Aqlan/issues/1#issue-3106821663


https://github.com/Aqlan1988/Aqlan/issues/1#issue-3106821663
