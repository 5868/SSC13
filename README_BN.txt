SSC13 GitHub Pages + Apps Script starter

1) Google Sheet-এর Extensions > Apps Script-এ Code.gs সম্পূর্ণ replace করুন।
2) Save করুন; setupDatabase() একবার Run করুন। Sheet1-এর A1:D1 header হতে হবে:
   ক্রমিক | নাম | গ্রাম | ফোন
3) Project Settings > Script Properties-এ ADMIN_PIN নামে কমপক্ষে 8 অক্ষরের secret PIN দিন।
4) Deploy > New deployment > Web app:
   Execute as: Me
   Who has access: Anyone
   Deploy করুন।
5) নতুন index.html খুলে API_URL-এ আপনার /exec URL বসান।
6) GitHub repository SSC13-এ index.html upload/commit করুন।
7) Repository Settings > Pages > Deploy from a branch > main > /(root) > Save।
8) কোডে পরিবর্তন করলে Apps Script-এর Deploy > Manage deployments > Edit > New version > Deploy করুন।

গুরুত্বপূর্ণ:
- পুরোনো Apps Script deployment URL একই deployment edit করলে সাধারণত একই থাকে; নতুন deployment করলে URL বদলাতে পারে।
- Public directory-তে ফোন নম্বর শুধু সদস্যের স্পষ্ট সম্মতিতে প্রকাশ করুন।
- Admin PIN কখনো GitHub-এ লিখবেন না।
- Removal approval করলে Sheet1 থেকে row delete হবে। আগে backup রাখা উচিত।
