# Test Plan – QAStudio TestOpsFlow

## 1) Amaç
Uygulamanın temel fonksiyonlarının doğrulanması; özellikle yetkilendirme, workflow geçişleri ve veri tutarlılığı risklerinin kontrol altına alınması.

## 2) Test Kapsamı
### Kapsam İçi
- Auth (register/login, token doğrulama, unauthorized akış)
- Workspace & Project CRUD + üyelik yönetimi
- Issue CRUD + filtreleme
- Workflow status geçişleri
- Sprint oluşturma/başlatma/tamamlama
- Comment ekleme
- Aktivite kaydı (temel)

### Kapsam Dışı
- Yük/performans testleri
- Gelişmiş güvenlik testleri
- Dosya yükleme ve e-posta bildirimleri

## 3) Test Seviyeleri ve Türleri
- Manuel fonksiyonel testler (smoke + regression)
- API test otomasyonu (Postman/Newman)
- UI E2E testleri (Cypress)
- Backend unit/integration testleri (Sprint 1+)

## 4) Test Ortamı
- Local: Backend + Postgres (Docker), Frontend
- CI: GitHub Actions (API + UI testlerinin headless çalışması)

## 5) Riskler ve Öncelikler
- R1 (Yüksek): Yetkisiz erişim / rol bypass (Auth/Authorization)
- R2 (Yüksek): Hatalı workflow geçişleri (Done’a yanlış geçiş)
- R3 (Orta): Sprint/Issue ilişkisinde veri tutarsızlığı
- R4 (Orta): Filtreleme/pagination hataları
- R5 (Düşük): UI hizalama/UX problemleri

## 6) Çıkış Kriterleri
- Kritik akışlar %100 geçmeli: login, workspace create, project create, issue create, status change
- P1 bug olmamalı, P2 bug sayısı sınırlı olmalı
- API test suite CI’da yeşil olmalı

## 7) Test Deliverables
- Test senaryoları (docs/test-scenarios.md)
- İzlenebilirlik matrisi (docs/test-matrix.md)
- Bug raporları (docs/bug-reports.md)
- API test koleksiyonu (api-tests/)
- UI E2E testleri (ui-tests/)
