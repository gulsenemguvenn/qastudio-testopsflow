# Test Scenarios – (Smoke)

Aşağıdaki senaryolar minimum “çalışır ürün” (MVP) doğrulaması için kullanılacaktır.

| ID | Modül | Tip | Senaryo | Beklenen |
|---|---|---|---|---|
| TS-001 | Auth | Pozitif | Geçerli bilgilerle login | 200 + JWT döner |
| TS-002 | Auth | Negatif | Yanlış şifre ile login | 401 + hata mesajı |
| TS-003 | Auth | Negatif | Token olmadan workspace list | 401 |
| TS-004 | Workspace | Pozitif | Workspace oluşturma | 201 + workspaceId |
| TS-005 | Workspace | Negatif | USER rolü ile member ekleme | 403 |
| TS-006 | Project | Pozitif | Workspace altında project oluşturma | 201 + projectId |
| TS-007 | Issue | Pozitif | Issue oluşturma (Task) | 201 + issueId |
| TS-008 | Issue | Negatif | Zorunlu alan boş (title) | 400 validation |
| TS-009 | Workflow | Negatif | Kurala aykırı status change | 409/400 |
| TS-010 | Comment | Pozitif | Issue’ya yorum ekleme | 201 |
