# QAStudio – TestOpsFlow | Requirements 

## 1) Vizyon
QAStudio – TestOpsFlow; test süreçlerini merkeze alan, Jira benzeri bir TestOps platformudur.
Amaç, issue yönetimi + workflow + sprint + test otomasyonu entegrasyonlarını tek bir ürün altında birleştirmektir.

## 2) Kapsam (V1)
### Kapsam İçi (V1)
- Kullanıcı kayıt / giriş (JWT)
- Workspace oluşturma ve üye yönetimi
- Project oluşturma ve üye yönetimi
- Issue (Bug/Task/Story) oluşturma, listeleme, güncelleme, silme
- Workflow & status geçişleri
- Kanban board görünümü
- Sprint oluşturma, başlatma, tamamlama
- Issue yorumları (Comments)
- Aktivite kayıtları (Activity Log) – temel seviyede

### Kapsam Dışı (Şimdilik)
- Performans testleri (yük testleri)
- File attachment (dosya yükleme)
- E-posta bildirimleri
- Mobil uygulama

## 3) Roller
- ADMIN: Workspace/Project yönetebilir, yetkilendirme yapabilir.
- USER: Issue oluşturabilir ve üzerinde işlem yapabilir (yetkisine göre).

## 4) EPIC & User Stories
### EPIC-1: Authentication & Authorization
- US-01: Kullanıcı olarak kayıt olabilmeliyim.
- US-02: Kullanıcı olarak giriş yapabilmeliyim.
- US-03: Rol bazlı yetkilendirme (ADMIN/USER) uygulanmalıdır.
- US-04: Token geçersiz/expired ise kullanıcı yeniden girişe yönlendirilmelidir.

### EPIC-2: Workspace Management
- US-05: Workspace oluşturabilmeliyim.
- US-06: Workspace üyelerini listeleyebilmeliyim.
- US-07: Workspace’e üye ekleyebilmeliyim (ADMIN).
- US-08: Workspace’ten üye çıkarabilmeliyim (ADMIN).

### EPIC-3: Project Management
- US-09: Project oluşturabilmeliyim (workspace altında).
- US-10: Project üyelerini yönetebilmeliyim (ADMIN).
- US-11: Project detaylarını görüntüleyebilmeliyim.

### EPIC-4: Issue Management
- US-12: Issue oluşturabilmeliyim (Bug/Task/Story).
- US-13: Issue listeleyebilmeliyim (filtreleme ile).
- US-14: Issue güncelleyebilmeliyim.
- US-15: Issue silebilmeliyim (rol kuralları ile).
- US-16: Issue durumunu değiştirebilmeliyim (workflow kurallarına göre).

### EPIC-5: Workflow & Board
- US-17: Issue’lar status sütunlarına göre board’da gösterilmelidir.
- US-18: Status geçişleri kurallara bağlı olmalıdır (ör. Done’a sadece belirli roller).

### EPIC-6: Sprint Management
- US-19: Sprint oluşturabilmeliyim.
- US-20: Sprint başlatıp tamamlayabilmeliyim.
- US-21: Sprint raporu görüntüleyebilmeliyim (tamamlanan/kalan issue sayısı).

### EPIC-7: Comments & Activity
- US-22: Issue’ya yorum ekleyebilmeliyim.
- US-23: Önemli aksiyonlar aktivite kaydı olarak loglanmalıdır (status change, assignee change).
