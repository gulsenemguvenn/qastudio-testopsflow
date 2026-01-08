# QAStudio – TestOpsFlow

QAStudio – TestOpsFlow, yazılım projelerinde **test süreçlerini merkeze alan**
iş takibi, hata yönetimi ve sprint akışlarını yöneten
**Jira benzeri bir TestOps platformudur**.

Bu proje, **QA-first yaklaşımı** ile tasarlanmış olup;
gereksinim analizi, manuel test, API test otomasyonu, UI testleri
ve CI/CD entegrasyonlarını tek bir ürün çatısı altında birleştirmeyi amaçlar.

---

## 🎯 Projenin Amacı

- TestOps yaklaşımını gerçek bir ürün üzerinde uygulamak  
- QA bakış açısıyla gereksinim, test ve geliştirme süreçlerini entegre etmek  
- Full-stack geliştirme bilgisini korurken QA uzmanlığı sergilemek  
- Jira benzeri bir sistemin sade ama işlevsel bir versiyonunu geliştirmek  

---

## 🧩 Temel Özellikler (V1)

- Workspace & Project yönetimi  
- Issue takibi (Bug / Task / Story)  
- Workflow & status yönetimi    
- Issue yorumları (Comments)  
- Aktivite / değişiklik logları  
- QA dokümantasyonu ve test otomasyonları  

---

## 🛠 Kullanılan Teknolojiler

### Backend
- Java Spring Boot
- RESTful API
- PostgreSQL
- JWT Authentication
- Clean Architecture yaklaşımı

### Frontend
- Angular
- Feature-based UI mimarisi

### Test & QA
- Manuel Test (Test Plan, Test Senaryoları)
- API Test Otomasyonu (Postman / Newman)
- UI E2E Testleri (Cypress)
- CI/CD (GitHub Actions)

---

## 🧪 QA-First Yaklaşım

Bu proje, klasik “önce kod sonra test” yaklaşımı yerine:

1. Gereksinimlerin yazılması  
2. Test senaryolarının oluşturulması  
3. API sözleşmelerinin tanımlanması  
4. Geliştirme sürecinin başlatılması  
5. Otomasyon testleri ve CI entegrasyonu  

şeklinde **test odaklı** bir yaklaşımla ilerlemektedir.

---

## 📁 Repo Yapısı

```text
qastudio-testopsflow/
├── docs/                 # Gereksinimler, test planları, senaryolar
├── backend/              # Spring Boot backend
├── frontend/             # Angular frontend
├── api-tests/            # Postman / Newman API testleri
├── ui-tests/             # Cypress UI testleri
├── docker/               # Docker & docker-compose
└── .github/workflows/    # CI pipeline

---

## 👩‍💻 Geliştirici Notu

Bu proje, bir **QA / Test Mühendisi** bakış açısıyla
test edilebilirlik, izlenebilirlik ve kalite odağı gözetilerek
geliştirilmektedir.

Amaç, yalnızca çalışan bir uygulama değil;
**test edilebilir, sürdürülebilir ve gerçek hayata yakın**
bir ürün ortaya koymaktır.