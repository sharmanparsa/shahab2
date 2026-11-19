# هفت‌خان: دونده‌ی بام‌ها (Shahab)

بازی دوبعدی Canvas داخل Android WebView.

- بازی: `app/src/main/assets/index.html`
- اندروید: `app/src/main/java/ir/shahab/game/MainActivity.java` (پرداخت مایکت + ذخیرهٔ نسخهٔ دوم)
- ساخت APK: GitHub Actions (`.github/workflows/build-apk.yml`، `assembleRelease`)
- امضا: `app/release.keystore` (مخزن را خصوصی نگه دارید و کلید را هرگز عوض نکنید)

## نسخهٔ 1.6 — ارتقای گرافیکی
- رابط: دکمه‌ها با عمق و افکت فشردن، HUD و عنوان طلایی، ورود نرم پنجره‌ها
- کیفیت گرافیک Low / Medium / High (دکمهٔ «کیفیت» در صفحهٔ اصلی؛ پیش‌فرض خودکار)
- افکت‌ها روی سیستم ذرات موجود: گردوغبار پرش/فرود/دویدن، جرقهٔ ضربه، مرگ دشمن، فلش قرمز آسیب، نور ضربه، ذرات محیطی
- سایهٔ زمین برای قهرمان/دشمن/باس، له‌شدگی و کشیدگی هنگام فرود و پرش، نور نرم دور قهرمان (High)
- باس: هاله (بنفش، در نیمهٔ دوم نارنجی)، نوار جان با انیمیشن کاهش نرم و نام
- کد: `up1.js` (به‌صورت لایه روی توابع موجود؛ منطق بازی بدون تغییر)

## نسخهٔ 1.7 — اسپرایت‌های تصویری
- قهرمان‌ها (۵ نفر، ۸ ژست: ایستاده، ۴ فریم راه رفتن، پرش، آسیب، پرتاب)، ۷ باس خان و ۲۱ دشمن با تصویر جدید (`spr.js` و `spr_data.js`)
- اگر تصویر بارگذاری نشود، نقاشی برداری قبلی نمایش داده می‌شود
- باس‌های داستان‌های فرعی همان باس‌های هفت‌خان را به‌کار می‌برند

## v1.8
- اسپرایت چندفریمی دشمن‌ها و باس‌ها (راه رفتن، حمله، آسیب)
- دویدن طبیعی‌تر قهرمان و اندازه‌ی بزرگ‌تر حالت کوچک

## v1.9
- عنکبوت، خفاش، لاک‌پشت دریایی و اژدهای جدید (چندفریمی)

## v2.0
- دویدن و راه رفتن واقعی (چرخه‌ی فریم) برای هر ۵ قهرمان

## v2.1
- Fixed cut/leaking hero run & walk frames (Gordafarid, Sohrab), cleaned stand/jump, enemy and boss frames.

## v2.2
- Full 6-12 frame walk cycles for all 7 bosses (lion, ogre, dragon, sorceress, giant, red demon, white demon).

## v2.3
- Dedicated jump/stand poses restored; run/walk frames feet-aligned with steady torso; ground-animal step bob; cleaned stray fragments.

## v2.4
- Painted sprites + walk/attack/hurt for 7 side-tale bosses; new viper-in-jar sprite.

## v2.5
- موسیقی فایل‌محور: menu، city1-7 (۳ مرحلهٔ عادی هر شهر)، boss1-7 (فقط نبرد باس) با کراس‌فید و لوپ. نقشهٔ فرعی و باس‌های فرعی هنوز موسیقی ساخته‌شدهٔ برنامه را دارند.

## v2.6
- ادامهٔ موسیقی از همان لحظه بعد از مکث (Pause → Resume).

## v2.7
- موسیقی نقشه‌های فرعی (smap1-7) و باس‌های فرعی (sboss1-7).
