# NyroxHub Store [NyPay]

Պրոֆեսիոնալ, responsive frontend store NyroxHub Minecraft network-ի համար։ Plain HTML/CSS/JavaScript՝ առանց React-ի կամ build step-ի։

## Հնարավորություններ
- Կոչումներ և երեք տեսակի քեյսեր
- Որոնում, ֆիլտրեր, sorting
- LocalStorage shopping cart
- NyPay checkout UI՝ առանց կեղծ վճարումների
- Նորությունների համակարգ և local admin form
- SEO metadata, robots.txt, sitemap.xml
- Mobile navigation, toast-եր, modal-ներ և smooth scrolling

## Server
`mc.nyroxhub.sryze.cc`

## NyPay / backend
Frontend-ը պատրաստ է իրական payment API-ին միանալու համար։ `js/cart.js`-ում checkout-ը intentionally չի հայտարարում հաջողված վճարում։ `js/admin.js`-ում կա backend/Web Push integration point։ Իրական վճարումների և browser push notifications-ի համար պետք է ավելացնել անվտանգ backend/payment provider և service worker/push credentials։

## Deploy
GitHub Pages-ում կարող ես publish անել repository-ի `main` branch-ը։
