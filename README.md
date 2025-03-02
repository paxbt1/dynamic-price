# شرح تسک:

یک افزونه وردپرس ایجاد کنید که در صفحات محصول ووکامرس، قیمت محصول را علاوه بر واحد اصلی (دلار) به یوان چین (CNY) نمایش دهد. نرخ تبدیل باید از یک API دریافت شود.

## نیازمندی‌ها:

### ۱. دریافت نرخ ارز از API  
- استفاده از API سایت [www.exchangerate-api.com](https://www.exchangerate-api.com)  
- **Your API Key:** `07335b99ef50f6a8120749d1`  
- **Example Request:**  
https://v6.exchangerate-api.com/v6/07335b99ef50f6a8120749d1/latest/USD

- دریافت نرخ تبدیل **دلار به یوان** و ذخیره‌ی آن در یک **ترانزینت (Transient) وردپرس** برای بهینه‌سازی درخواست‌های API (مثلاً هر ۶۰ دقیقه یکبار به‌روزرسانی شود).

### ۲. نمایش قیمت به یوان در صفحات محصول ووکامرس  
- در **صفحه محصول (single product)**، قیمت به یوان محصول را در **زیر قیمت اصلی** نمایش دهید.  
- استفاده از **یک شورت‌کد** برای نمایش قیمت محصول به یوان در جای دلخواه.  
- استفاده از **CSS و JavaScript** برای **طراحی زیبا و نمایش داینامیک قیمت**.  

### ۳. دکمه "به‌روزرسانی قیمت به یوان" در ادمین وردپرس  
- افزودن گزینه‌ای در **تنظیمات افزونه** برای به‌روزرسانی دستی نرخ ارز.  
- استفاده از **AJAX و REST API وردپرس** برای ارسال درخواست به API و **به‌روزرسانی نرخ ارز بدون نیاز به رفرش صفحه**.  
