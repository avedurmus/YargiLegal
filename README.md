# Yargı Legal Assistant - Claude.ai Projects Şablonları

Bu dizin, kendi hukuk büronuzda veya kurumsal hukuk departmanınızda kullanabileceğiniz, **Claude.ai Projects** tabanlı hibrit bir hukuk asistanı kurmanız için gerekli şablonları içerir.

Anthropic'in açık kaynaklı `claude-for-legal` referans paketinden türetilen ve Türk hukukuna uyarlanan bu sistem, iki ana şablon sunmaktadır:

---

## 📁 Dizin Yapısı

*   **[Law-Firm-Assistant](file:///Users/emredurmus/Documents/YargiMCP/YargiLegal-Assistant/Law-Firm-Assistant/) (Hukuk Büroları İçin):** Dava ve hukuki danışmanlık süreçlerini (15 pratik alan, dava yönetimi, süre takip, UYAP entegrasyonu vb.) kapsayan kapsamlı şablon.
*   **[Corporate-Assistant](file:///Users/emredurmus/Documents/YargiMCP/YargiLegal-Assistant/Corporate-Assistant/) (Kurumsal Hukuk Departmanları İçin):** Şirket içi hukuk departmanlarının sözleşme redline, KVKK/gizlilik, regülasyon takibi ve şirket içi süreçlerini yöneten şablon.

Her iki dizin de kendi içinde şu standart yapıyı barındırır:
*   `SYSTEM_PROMPT.md`: Claude.ai Project'inizin **Custom Instructions** alanına ekleyeceğiniz sistem talimatı.
*   `KURULUM.md`: Adım adım Türkçe kurulum kılavuzu.
*   `INSTALLATION.md`: Adım adım İngilizce kurulum kılavuzu.
*   `knowledge/`: Claude.ai Project'inizin **Knowledge** bölümüne yüklenecek olan md dosyaları (playbook'lar, referanslar ve kurallar).

---

## 🚀 Hızlı Kurulum Adımları

Hukuk Bürosu veya Kurumsal Asistan şablonlarından hangisini kullanmak istiyorsanız, ilgili klasörün içindeki `KURULUM.md` dosyasını açıp adımları izleyin. Genel kurulum akışı şu şekildedir:

1.  **Project Oluşturun:** [claude.ai](https://claude.ai) üzerinde yeni bir **Project** açın.
2.  **Sistem Talimatı (Custom Instructions):** `SYSTEM_PROMPT.md` dosyasının içeriğini kopyalayarak projenizin **Customize** -> **Custom Instructions** bölümüne yapıştırın.
3.  **Knowledge Yükleyin:** `knowledge/` klasörünün içindeki dosyaları (ana profil, pratik alan profilleri, skill ve reference dosyalarını) projenizin **Knowledge** alanına yükleyin.
4.  **TR Legal MCP Bağlantısı (Önerilir):** Proje ayarlarına `yargi-mcp-pro` sunucu bağlantısını ekleyin.
5.  **Profilinizi Doldurun:** Claude arayüzünde ilk konuşmada `/firm-operations:cold-start-interview` (veya kurumsal asistan için `/company-operations:cold-start-interview`) komutunu çalıştırarak sistemin sizin çalışma profilinizi interaktif olarak öğrenmesini sağlayın.

---

## ✍️ Özelleştirme ve Markalama

Eğer bu şablonları kendi firmanızın adına (örn. "ArthurLegal" yerine "YargıLegal" veya kendi büro/şirket isminizle) markalamak isterseniz:

1.  `SYSTEM_PROMPT.md` dosyalarındaki `ArthurLegal` ifadelerini kendi isminizle değiştirin.
2.  `knowledge/firm-profile.md` veya `knowledge/company-profile.md` dosyasındaki default büro/şirket adını kendinize göre güncelleyin.

*Not: Şablonlardaki özelleştirilebilir alanlar `[DOLDUR]` veya `[FILL]` şeklinde işaretlenmiştir.*

---

## ⚖️ Lisans ve Atıf

Bu şablonlar **Apache License 2.0** altında lisanslanmıştır. Kendi ticari veya bireysel süreçleriniz için özelleştirebilir, kopyalayabilir ve kullanabilirsiniz. Orijinal atıf dosyalarını (`ATTRIBUTION.md` ve `LICENSE`) dizinlerde korumanız gerekmektedir.
