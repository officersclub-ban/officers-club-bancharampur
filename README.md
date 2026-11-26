# অফিসার্স ক্লাব বাঞ্ছারামপুর

সদস্য তথ্য ও মাসিক চাঁদা ব্যবস্থাপনার একটি একক-ফাইল HTML অ্যাপ (Firebase Firestore + Hosting)।

## ফাইল
- `public/index.html` — ক্লাবের পাবলিক ওয়েবসাইট (পরিচিতি, কমিটি, নোটিশ, সদস্যের নাম, যোগাযোগ)
- `public/admin.html` — অ্যাডমিন ও চাঁদা ব্যবস্থাপনা অ্যাপ
- `firestore.rules` — Firestore নিরাপত্তা নিয়ম
- `firebase.json` — Hosting ও Firestore কনফিগ

## চালু করার ধাপ
1. Firebase প্রজেক্ট খুলে Firestore ও Email/Password Authentication চালু করুন।
2. `public/admin.html` ও `public/index.html` দুটোরই ওপরের `firebaseConfig`-এ নিজের প্রজেক্টের তথ্য বসান।
3. `firebase login` তারপর `firebase deploy`।

## সতর্কতা
- এসএমএস গেটওয়ের API কী বা পাসওয়ার্ড কখনো কোডে লিখে কমিট করবেন না; সেটি অ্যাপের সেটিংস থেকে দিন।
- সদস্যদের মোবাইল নাম্বারসহ কোনো ডেটা ফাইল (CSV/এক্সেল) রিপোজিটরিতে রাখবেন না।
