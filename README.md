# אתר מדיניות הפרטיות של FixGo

תיקייה זו מכילה אתר סטטי עצמאי (`index.html`) עם מדיניות הפרטיות של FixGo
בארבע שפות (עברית, אנגלית, רוסית, ערבית) + מתג שפה.

האתר משמש כדי לקבל **כתובת URL ציבורית** למדיניות הפרטיות — דרישה חובה
בעת הגשת האפליקציה ל-App Store / Google Play.

## אפשרות 1: פריסה עם GitHub Pages (מומלץ, חינמי)

1. צרו ריפו חדש בגיטהאב (פרטי או ציבורי — לא משנה), לדוגמה: `fixgo-privacy-policy`.
2. העלו את הקובץ `index.html` מהתיקייה הזו לתיקיית הבסיס (root) של הריפו.
3. בריפו, היכנסו ל: **Settings → Pages**.
4. תחת "Build and deployment", בחרו:
   - Source: **Deploy from a branch**
   - Branch: **main** (או `master`), תיקייה: **/ (root)**
5. שמרו. אחרי כ-1-2 דקות תקבלו כתובת בפורמט:
   ```
   https://<your-github-username>.github.io/fixgo-privacy-policy/
   ```
6. זו הכתובת שיש להזין ב-App Store Connect / Google Play Console כ-Privacy Policy URL,
   וגם להחזיר אליי כדי שאוסיף קישור אליה מתוך מסך "הגדרות" באפליקציה (אם תרצו קישור חיצוני בנוסף למסך הפנימי).

## אפשרות 2: פריסה עם Netlify (גם חינמי, גם פשוט)

1. נכנסים ל-https://app.netlify.com (אפשר עם חשבון Google/GitHub).
2. "Add new site" → "Deploy manually".
3. גוררים את התיקייה הזו (או רק את `index.html`) לאזור ההעלאה.
4. Netlify ייתן כתובת אקראית בפורמט `https://<random-name>.netlify.app` —
   ניתן לשנות את השם ב-Site settings → Change site name.

## עדכון תוכן בעתיד

אם מדיניות הפרטיות תשתנה, יש לעדכן גם:
- את הקובץ `index.html` בתיקייה זו (ולפרוס מחדש),
- ואת `legal.privacyPolicy` בקבצי `src/locales/{he,en,ru,ar}/common.json`
  (המסך הפנימי באפליקציה, בנתיב `/privacy-policy`).

שני המקומות צריכים להישאר זהים בתוכן.
