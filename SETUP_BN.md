# Medical Visa Undertaking Generator - সেটআপ গাইড

## কী করতে হবে?

এই ওয়েবসাইট সম্পূর্ণ **free** এবং **lifetime** ব্যবহার করা যাবে কোনো খরচ ছাড়াই।

---

## Step-by-Step সেটআপ (সবচেয়ে সহজ - Vercel)

### Step 1: GitHub একাউন্ট খোলো
- https://github.com/signup এ যাও
- Email, password দিয়ে sign up করো

### Step 2: Repository তৈরি করো
- GitHub এ যাও → "New Repository" ক্লিক করো
- Repository name: `medical-visa-gen`
- "Create repository" ক্লিক করো

### Step 3: ফাইল আপলোড করো
GitHub-এ:
```
Upload করো:
├── index.html
├── README.md
├── SETUP_BN.md
├── .gitignore
└── assets/ folder
```

Git command (যদি terminal জানো):
```bash
git init
git add .
git commit -m "Initial upload"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/medical-visa-gen.git
git push -u origin main
```

### Step 4: Vercel-এ Deploy করো
1. https://vercel.com এ যাও
2. "Sign Up" → GitHub এর মাধ্যমে করো
3. "Import Project" ক্লিক করো
4. নিজের `medical-visa-gen` repository সিলেক্ট করো
5. "Deploy" ক্লিক করো

**Done!** তোমার সাইট live হবে:
```
https://medical-visa-gen.vercel.app
```

---

## সম্পূর্ণ সম্পদ খরচ: $0 ✅

| সেবা | খরচ | কেন |
|------|------|-----|
| Vercel | Free | Unlimited hosting |
| GitHub | Free | Code storage |
| Custom Domain | ~$3-15/year | Optional (তোর ডোমেইন ব্যবহার করতে পারবি) |

---

## নিজের Domain ব্যবহার করতে চাইলে

**যদি `yourdomain.com` আছে:**

Vercel Settings-এ:
1. "Domains" → "Add Domain"
2. `yourdomain.com` লিখো
3. DNS settings দেখো (cPanel-এ CNAME add করো)

---

## কোনো সমস্যা হলে

### ফাইল মিসিং?
নিশ্চিত করো folder structure ঠিক আছে:
```
medical-visa-gen/
├── index.html
├── assets/
│   ├── js/
│   │   ├── app.js
│   │   └── tsaf-promo.js
│   ├── css/
│   │   └── bengali.css
│   └── vendor/
│       ├── pdf.min.js
│       ├── pdf-lib.min.js
│       └── qrcode.min.js
```

### Deploy এ error?
- Vercel logs দেখো
- `.gitignore` আছে কি দেখো
- Repository public কি দেখো

---

## ভবিষ্যতে কোনো বদল করতে চাইলে

1. ফাইল edit করো (local machine-এ)
2. GitHub-এ push করো:
   ```bash
   git add .
   git commit -m "Your change"
   git push
   ```
3. Vercel auto-redeploy হবে (2-3 মিনিট)

---

## কেন এটা free?

- **Vercel**: হাজার হাজার free projects host করে
- **GitHub**: ১০০% free code hosting
- **কোনো database নেই**: সব কাজ browser-এ হয়

---

## আরো সাহায্য প্রয়োজন?

- Vercel docs: https://vercel.com/docs
- GitHub docs: https://docs.github.com
- এই README.md ফাইলটা পড়ো

**খরচ: $0 | সময়: ৫ মিনিট | চিরকাল ব্যবহার করতে পারবি ✅**
