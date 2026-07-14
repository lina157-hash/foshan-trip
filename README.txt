佛山之旅｜Firebase 雲端同步版

上傳方式：
1. 解壓縮 ZIP。
2. 到 GitHub 儲存庫 lina157-hash/foshan-trip。
3. Add file → Upload files。
4. 上傳本資料夾內的 index.html、manifest.json、service-worker.js、icon-192.png、icon-512.png，覆蓋舊檔。
5. Commit changes。
6. 等候 GitHub Pages 重新部署，開啟 https://lina157-hash.github.io/foshan-trip/

首次使用：
1. 打開網站，按「管理員登入」。
2. 輸入 Firebase Authentication 建立的 Email 與密碼。
3. 若 Firestore 尚無 trips/foshan2026，系統會自動建立第一份雲端資料。
4. 之後每次修改都會自動同步，其他裝置會即時更新。

安全：
- firebaseConfig 可放在前端；寫入權限由 Authentication 與 Firestore Rules 控制。
- 不要把管理員密碼上傳 GitHub 或傳給他人。
- Firestore 規則必須只允許指定 UID 寫入。


本版已將同行人數改為 7 人，並會在管理員登入後把既有 6 人雲端資料自動補上「旅伴 7」。共同記帳的平均每人金額會依旅伴名單人數自動計算。
