AinPath Update Source — GitHub-ready package

এই ফোল্ডারটি public GitHub repository হিসেবে publish করুন। প্রস্তাবিত repository নাম:
ainpath-updates

১) update.json খুলে YOUR_GITHUB_USERNAME জায়গায় আপনার GitHub username বসান।
২) পুরো ফোল্ডারটি repository-র main branch-এ upload/push করুন।
৩) তারপর AinPath Control Center → Settings → Update Manifest URL-এ দিন:
https://raw.githubusercontent.com/YOUR_GITHUB_USERNAME/ainpath-updates/main/update.json
৪) Save করুন।
৫) Update Center → Check Now চাপুন।

ভবিষ্যৎ update প্রকাশের নিয়ম:
- নতুন ZIP packages/ ফোল্ডারে দিন।
- update.json-এ version, download_url, changelog এবং sha256 বদলান।
- Commit/push করুন।
- AinPath দিনে দুইবার source check করবে; নতুন version হলে Notifications-এ দেখাবে।

নিরাপত্তা নোট:
বর্তমান AinPath 2.2.0 manifest-এর sha256 field সংরক্ষণ করতে পারে, কিন্তু installer এখনো sha256 enforce করে না। ভবিষ্যৎ core update-এ checksum verification enforce করা যেতে পারে।
