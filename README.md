# পুস্তক PWA — GitHub Pages + PWABuilder

## ১. GitHub-এ আপলোড
1. github.com → New repository (নাম যেমন `pustok`), **Public**।
2. "uploading an existing file" চেপে এই ফোল্ডারের **ভেতরের সব ফাইল ও ফোল্ডার** (index.html, sw.js, manifest.webmanifest, icons/, screenshots/, .nojekyll) টেনে আনুন। `index.html` অবশ্যই রিপোজিটরির root-এ থাকতে হবে।
3. Commit করুন।
4. Settings → Pages → Source: **Deploy from a branch** → Branch: `main` / `(root)` → Save।
5. ১-২ মিনিট পর লিংক পাবেন: `https://YOUR-USERNAME.github.io/pustok/`

## ২. প্রথমবার অনলাইনে একবার খুলুন
লিংকটি ফোনের Chrome-এ ইন্টারনেট সহ একবার খুলুন। এতে অ্যাপ ও ফন্ট/লাইব্রেরি ফাইল ক্যাশ হয়, এরপর অফলাইনেও চলবে।

## ৩. PWABuilder
1. pwabuilder.com → উপরের লিংক বসিয়ে Start।
2. Manifest ও Service Worker দুটোই সবুজ দেখাবে। Android / Windows প্যাকেজ বানান।

## আপডেট দিলে
`sw.js`-এর `VERSION = 'pustok-v1'` বদলে `pustok-v2` করুন, নইলে ফোনে পুরনো ক্যাশ থাকবে।

## আপডেট v2 (এই সংস্করণে ঠিক করা হয়েছে)
- বই সেভ হচ্ছিল না: বড় ছবি (ফোনের ক্যামেরা ফটো) স্টোরেজ ভরে ফেলছিল। এখন ছবি আপলোডের সময় স্বয়ংক্রিয়ভাবে ছোট করা হয়, আর সেভ ব্যর্থ হলে স্পষ্ট বার্তা দেখায়।
- স্ট্যাটাস ব্যাজ এখন ছবির নিচে।
- তারিখের নিয়ম: পড়া হয়নি/উইশলিস্ট = কোনো তারিখ নয়, পড়ছি = শুধু শুরুর তারিখ, পড়া শেষ = শুরু ও শেষ।
- পুরনো সেভ করা বইয়ের তারিখ ও বড় ছবি প্রথমবার খোলার সময় নিজে ঠিক হয়ে যাবে।
- GitHub-এ সব ফাইল আবার আপলোড করে (replace) Commit করুন। ফোনে অ্যাপ একবার বন্ধ করে খুললে নতুন সংস্করণ চালু হবে।
