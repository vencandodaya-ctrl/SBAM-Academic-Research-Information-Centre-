# SBAM Mobile — GitHub Pages PWA

ဒီ folder ကို GitHub repository ထဲကို တင်ပြီး GitHub Pages ဖြင့် publish လုပ်နိုင်ပါတယ်။

## ပါဝင်တဲ့ဖိုင်များ

- `index.html` — ပြင်ပြီးသား SBAM Mobile main page
- `manifest.webmanifest` — PWA install configuration
- `manifest.json` — manifest configuration copy
- `sw.js` — Service Worker / offline cache
- `icons/icon-192.png` — Android/PWA icon
- `icons/icon-512.png` — Android/PWA icon
- `.nojekyll` — GitHub Pages static-file compatibility
- `README.md` — ဒီလမ်းညွှန်

## GitHub Pages

1. GitHub မှာ repository အသစ်တစ်ခုဖန်တီးပါ။
2. ဒီ folder ထဲက ဖိုင်/ဖိုလ်ဒါအားလုံးကို repository ရဲ့ root ထဲ upload လုပ်ပါ။
3. Repository → **Settings → Pages**
4. **Deploy from a branch** ကိုရွေးပါ။
5. Branch = `main`, Folder = `/ (root)` → Save.
6. GitHub က ပေးတဲ့ `https://...github.io/.../` link ကို ဖွင့်ပါ။
7. Android Chrome မှာ **Install app / Add to Home screen** ကိုရွေးနိုင်ပါမယ်။

### အရေးကြီး
PWA install အတွက် HTTPS လိုအပ်ပါတယ်။ GitHub Pages က HTTPS ပေးတဲ့အတွက် ဒီအတွက် သင့်တော်ပါတယ်။

`sw.js` က update လုပ်တိုင်း `CACHE_NAME` ရဲ့ version (`v1`, `v2`, `v3`...) ကို တိုးပေးရင် browser cache ဟောင်းကို အစားထိုးနိုင်ပါတယ်။
