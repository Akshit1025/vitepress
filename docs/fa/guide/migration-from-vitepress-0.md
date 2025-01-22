# مهاجرت از ویت‌پرس 0.x

اگر از نسخه 0.x ویت‌پرس می‌آیید، تغییرات قابل توجهی به دلیل ویژگی‌ها و بهبودهای جدید وجود دارد. لطفاً این راهنما را دنبال کنید تا ببینید چگونه برنامه خود را به ویت‌پرس جدیدتر منتقل کنید.

## پیکربندی برنامه

- ویژگی بین‌المللی‌سازی هنوز اجرا نشده است.

## پیکربندی تم

- گزینه `sidebar` ساختار خود را تغییر داده است.
  - کلید `children` حالا به نام `items` نامیده می‌شود.
  - در حال حاضر ممکن است مورد بالادستی حاوی `link` نباشد. ما قصد داریم این گزینه را بازگردانیم.
- `repo`، `repoLabel`، `docsDir`، `docsBranch`، `editLinks`، `editLinkText` به منظور API انعطاف‌پذیرتر حذف شده‌اند.
  - برای اضافه کردن لینک GitHub با آیکون به نوار ناوبری، از ویژگی [پیوندهای اجتماعی](../reference/default-theme-nav#navigation-links) استفاده کنید.
  - برای اضافه کردن ویژگی "ویرایش این صفحه"، از ویژگی [پیوند ویرایش](../reference/default-theme-edit-link) استفاده کنید.
- گزینه `lastUpdated` حالا به `config.lastUpdated` و `themeConfig.lastUpdatedText` تقسیم شده است.
- `carbonAds.carbon` به `carbonAds.code` تغییر کرده است.

## پیکربندی Frontmatter

- گزینه `home: true` به `layout: home` تغییر کرده است. همچنین، تنظیمات مربوط به صفحه اصلی بسیار تغییر کرده‌اند تا ویژگی‌های اضافی را ارائه دهند. برای جزئیات بیشتر، [راهنمای صفحه اصلی](../reference/default-theme-home-page) را ببینید.
- گزینه `footer` به [`themeConfig.footer`](../reference/default-theme-config#footer) منتقل شده است.