---
name: mikra
description: |
  הקשר פרויקט מקרא. הפעל כשעובדים על mikra-system, mikrabooks, או כל קוד הקשור לעסק.
  Use when: building UI components, adding features, modifying styles, or reviewing code for this project.
allowed-tools: Read Grep Glob Bash Edit Write
---

# הקשר פרויקט – מקרא הוצאה לאור

## מה המערכת
מערכת ניהול עסקית לבית דפוס מקרא בשותפות עם יפה נוף (50/50).

## סטאק טכני
- **Frontend**: HTML/CSS/JS וניל – אין framework
- **Backend**: Google Apps Script (Web App)
- **Hosting**: GitHub Pages
- **UI**: RTL, עברית, dark sidebar

## עקרונות UI
- **תמיד RTL**: `<html lang="he" dir="rtl">`
- **פונטים**: Heebo (גוף) + Frank Ruhl Libre (כותרות)
- **צבעים**:
  - Primary: `#1a2f4a` (כחול כהה)
  - Accent: `#c8913a` (זהב)
  - Dark bg: `#111b28`
- **Sidebar**: כהה עם ניווט מודולים
- CSS variables – תמיד השתמש במשתנים הקיימים, אל תוסיף ערכים קשיחים

## מבנה העסק
- שותפות 50/50: מקרא ↔ יפה נוף
- חלוקת רווח לפי סוג עבודה: פריסה / גרפיקה / הדפסה / עריכה / חיוב ישיר
- ביינוש = שותף + לפעמים ספק (שני מצבים נפרדים)

## מודולים קיימים
- ניהול לקוחות
- הצעות מחיר
- מעקב פרויקטים
- היסטוריית תשלומים
- ניהול משימות (`tasks.html`)
- פיננסים אישיים (`personal-finance.html`)
- ייצוא PDF, קישור Dropbox, אינטגרציית WhatsApp

## כללי ברזל לפני כל שינוי
1. **קרא קודם** – תמיד קרא את הקובץ הרלוונטי לפני עריכה
2. **אל תשבור** – לא לגעת בפונקציונליות קיימת שאינה קשורה לשינוי
3. **עקביות סגנון** – כל דף חדש חייב להיראות כמו שאר הדפים
4. **JS וניל** – אין jQuery, אין React, אין framework
5. **עברית בממשק** – כל טקסט משתמש בעברית, כולל הודעות שגיאה

## תבנית דף HTML חדש
```html
<!DOCTYPE html>
<html lang="he" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[שם הדף] | מקרא</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link href="https://fonts.googleapis.com/css2?family=Heebo:wght@300;400;500;600;700&family=Frank+Ruhl+Libre:wght@400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- sidebar + main content -->
</body>
</html>
```

## מה עכשיו פתוח בריפו
!`ls /home/user/mikrabooks/*.html 2>/dev/null || echo "רק index.html"`
