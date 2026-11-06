# Steward: Fikir Analizi ve Rekabet Araştırması

**Tarih:** 2026-11-06
**Bu dosyanın rolü:** Roadmap, Mimari ve Pazar araştırması dokümanlarındaki fikri dışarıdan değerlendirir. Varsayımları web araştırmasıyla kontrol eder. Güçlü ve zayıf yönleri, SWOT ve diğer çerçeveleri, güncel rekabet haritasını ve tartışılacak kararları içerir.
**Kaynak dokümanlar:** `2026-11-06-Roadmap.md`, `2026-11-06-Mimari.md`, `2026-11-06-OnPremAI-research.md`, `2026-11-06-PulsElektronik-gorusme.md`

---

## 0. Özet

Fikir sağlam bir acıya oturuyor: KVKK gölge AI'ı adıyla andı, çalışanlar AI'ı kullanıyor, şirketlerin politikası yok. Mimari (lokal maskele, buluta gönder, geri doldur) doğru. Ama dokümanlardaki iki varsayım yanlış çıktı:

1. **"Orta (KOBİ ekibi + Türkçe + KVKK) boş görünüyor" varsayımı doğru değil.** Ankara merkezli AltaySec'in **Guardian Edge** ürünü aynı işi yapıyor: Chrome eklentisi, TC kimlik ve IBAN maskeleme, şirket sözlüğü, geri doldurma, shadow mode, KVKK dili. Pilot aşamasında ve fiyatı yok. Global tarafta **PiiBlocker** koltuk başına 4,99–6,99 USD'ye admin paneli, GPO kurulumu ve geri doldurma veriyor.
2. **"Alt tarafta ücretsiz tek kişilik eklentiler" varsayımı eksik.** Alt taraf artık ücretli, ekip yönetimli ve ucuz. UK'de **ChatShield** hukuk ve muhasebe büroları için kullanıcı başı 8–15 GBP alıyor. Bu, dokümandaki GB planının (UK regüle meslekler) zaten dolu olduğunu gösterir.

Buna karşılık üç şey hâlâ boş ve Steward'ın gerçek farkı olabilir:

- **KVKK kanıt çıktısı:** Kurum'un istediği politika, erişim kuralı ve kayıt dosyasını hazır rapor olarak veren bir KOBİ ürünü yok.
- **Türk ERP sözlüğü ve Türkçe NER:** Rakiplerin hiçbiri Logo/Mikro/Netsis cari listesinden sözlük çıkarmıyor.
- **Gizliliği koruyan verim katmanı:** Departman bazlı AI fırsat haritasını KOBİ için kimse yapmıyor. Kurumsalda Harmonic "Usage Intelligence" ile aynı yöne gidiyor.

**Tavsiye:** Fikre devam. Ama konumu "gölge AI kalkanı" değil, **"KVKK kanıtı + verim haritası"** olarak kur. Kalkan mekanizması ucuzlaşan bir özellik, kanıt ve verim ise satın alma nedeni. Skor kartı 22/40'tan **26/40**'a çıkıyor (bkz. bölüm 11).

---

## 1. Dokümanlardaki varsayımların kontrolü

| Varsayım (dokümanlarda) | Durum | Bulgu |
| :--- | :--- | :--- |
| KVKK 5 Mart 2026'da gölge AI duyurusu yaptı | ✅ Doğru | Duyuru "İş Yerlerinde Üretken Yapay Zekâ Araçlarının Kullanımı" başlığıyla yayımlandı; politika, onaylı araç listesi ve farkındalık öneriyor ([ACR Legal](https://ayseeceacar.av.tr/kvkk-uyardi-is-yerinde-golge-yapay-zeka-kullanmak-artik-risk-cursor-ve-kimi-davasi-ne-gosteriyor/), [Anka Law](https://www.anka.law/makaleler/kisisel-verileri-koruma-kurumunun-yeni-dokumani-isiginda-golge-yapay-zeka/)) |
| KVKK ilke kararı 2026/2035 sürekli izlemeyi yasaklıyor | ✅ Doğru | 16 Eylül 2026 tarihli karar 8 Ekim'de Resmî Gazete'de çıktı. Denetim meşru amaçla sınırlı ve ölçülü olmalı, çalışan önceden aydınlatılmalı ([Erdem & Erdem](https://www.erdem-erdem.av.tr/bilgi-bankasi/kurumsal-iletisim-araclarinin-denetlenmesine-iliskin-ilke-karari-yayimlandi), [Forbes TR](https://www.forbes.com.tr/haberler/isverenler-artik-calisanlarin-e-postalarini-gizlice-denetleyemeyecek)) |
| Copilot Türkiye'de ülke içi işleme sunmuyor | ✅ Doğru, hatta güçlendi | Microsoft Nisan 2026'da listeyi daralttı. 2026 sonu: Avustralya, Hindistan, BAE, UK, ABD. Kanada 2027, Japonya 2028. Almanya ve diğerleri tarihsiz. Türkiye hiçbir listede yok ([Microsoft](https://www.microsoft.com/en-us/microsoft-365/blog/2025/11/04/microsoft-offers-in-country-data-processing-to-15-countries-to-strengthen-sovereign-controls-for-microsoft-365-copilot/)) |
| TÜİK: şirketlerde AI kullanımı %14 | ✅ Doğru, ayrıntı eklendi | 2026: 10–49 çalışan %12,8; 50–249 çalışan %17,0; 250+ %37,1. 2025'te genel %7,5 idi ([Quasa/TÜİK](https://quasa.io/tr/media/turkiyede-sirketlerin-ai-kullanimi-ikiye-katlandi-insaat-yuzde-69da-kaldi)) |
| Harmonic 50M USD Series B, Ekim 2026 | ✅ Doğru | 14 Ekim 2026, Crosspoint Capital. 100+ kurumsal müşteri. "Usage Intelligence" katmanı hangi AI kullanımının değer ürettiğini gösteriyor ([Unite.AI](https://unite.ai/harmonic-security-raises-50m-series-b-to-expand-us-and-uk-teams)) |
| SentinelOne → Prompt Security, Check Point → Lakera | ✅ Doğru | Prompt Security Ağustos 2025, 250–300M USD tahmini ([SiliconANGLE](https://siliconangle.com/2025/08/05/sentinelone-acquires-ai-security-startup-prompt-security/)). Lakera Eylül 2025, ~300M USD ([SecurityWeek](https://www.securityweek.com/check-point-to-acquire-ai-security-firm-lakera/)) |
| Perplexity Hybrid Compute mekanizmayı doğruladı | ✅ Doğru | 1 Eylül 2026, sadece Apple silicon Mac ([Unite.AI](https://www.unite.ai/perplexity-launches-hybrid-compute-on-mac-with-local-privacy-gate/)) |
| Orta segment (KOBİ + Türkçe + KVKK) boş | ❌ Yanlış | AltaySec **Guardian Edge** (Ankara) aynı segmentte, pilot aşamasında ([AltaySec](https://altaysec.com.tr/urunler/guardian-edge)) |
| Alt tarafta sadece ücretsiz tek kişilik eklentiler var | ❌ Eksik | PiiBlocker (4,99–6,99 USD/koltuk, admin paneli, GPO), ChatShield (8–15 GBP/kullanıcı), ShadowLock (cihaz başı, MSP) ([PiiBlock](https://www.piiblock.com/), [Capterra](https://www.capterra.com/p/10044878/ChatShield/)) |
| LayerX bağımsız bir rakip | ⚠️ Değişti | Akamai, LayerX'i Mayıs 2026'da 205M USD'ye satın aldı ([haber](https://the-coders-blog.pages.dev/akamai-buys-layerx-a-205m-bet-on-ai-browser-security/)) |
| Chrome Enterprise Premium pahalı ve kurumsal | ⚠️ Kısmen | Liste fiyatı kullanıcı başı aylık **6 USD**. Satış "uzmanla konuş" üzerinden ([Chrome Enterprise](https://chromeenterprise.google/intl/ko/pricing/)) |
| Steward adı GB'de AML şirketiyle çakışıyor | ✅ Doğru | getsteward.ai, New York ve Londra, 5M USD, Mart 2026, Motive Partners ([tech.eu](https://tech.eu/2026/03/17/steward-an-ai-driven-compliance-platform-managing-100b-raises-5m/)) |

---

## 2. Güçlü yönler

1. **Düzenleyici zamanlama gerçek.** KVKK'nın Mart 2026 gölge AI duyurusu satış cümlesini hazır veriyor. 2026/2035 ilke kararı "log gibi az müdahaleci yöntem" diyerek Steward'ın metadata-only tasarımını açıkça meşrulaştırıyor. Teramind tipi ekran kaydı araçları bu kararla Türkiye'de hukuken zorlaşıyor; Steward kazançlı çıkıyor.
2. **Ceza çapası yüksek.** 2026'da veri güvenliği ihlali cezası 256.357–17.092.242 TL. Yurt dışı aktarım standart sözleşmesini bildirmeme cezası 90.308–1.806.377 TL ([CottGroup](https://cottgroup.com/tr/mevzuat/item/yeniden-degerleme-oranina-gore-2026-yili-kvkk-idari-para-cezalari)). Yıllık birkaç bin dolarlık bir ürün, alt sınırın bile çok altında.
3. **İçerik sunucuya hiç gelmiyor.** Bu, Türkiye'deki tek rakip Guardian Edge'den daha iyi bir gizlilik hikâyesi. Guardian Edge içeriği müşterinin Guardian sunucusunda tarıyor; Steward tarayıcıda tarıyor. "Bize bile güvenmek zorunda değilsiniz" satır satır doğrulanabilir (giden metin görünümü, kanarya testi).
4. **Maskele + geri doldur, engelle değil.** Chrome Enterprise Premium ve Edge + Purview sadece engelliyor veya denetliyor; maskeleme yok ([Microsoft Learn](https://learn.microsoft.com/en-us/purview/dlp-browser-dlp-learn)). Engelleme çalışanı telefona kaçırır, maskeleme işini bitirtir. Bu, benimseme için kritik.
5. **Türkiye'ye özgü tespit.** TC kimlik, VKN, IBAN, SGK doğrulamalı kurallar; Logo/Mikro/Netsis cari listesi; Türkçe NER. Global rakiplerin hiçbirinde yok. Guardian Edge'de TC ve IBAN var ama ERP sözlüğü yok.
6. **Verim katmanı, gizlilik koruyarak.** Patron için ürün "maliyet" değil "fırsat". Rakiplerde ya hiç yok (PiiBlocker, ChatShield, Guardian Edge) ya kurumsal (Harmonic) ya da gözetleme tipi (ActivTrak, Insightful).
7. **Sıcak ilk müşteri ve düşük sermaye.** Puls pilotu, tek geliştirici, donanım yok. Faz 0 için 2–3 hafta gerçekçi.
8. **Çıkış pazarı sıcak.** Akamai–LayerX (205M), SentinelOne–Prompt Security (~250M), Check Point–Lakera (~300M), Harmonic Series B (50M). Alıcılar tarayıcı katmanını satın alıyor.

## 3. Zayıf yönler

1. **Mekanizma meta oldu.** Lokal maskeleme + geri doldurma artık PiiBlocker'da ücretsiz, Guardian Edge'de pilot, Perplexity'de ürün içi. Bunu "ürün" diye satmak zor. Ürün = kanıt + verim + yerel sözlük olmalı.
2. **Fiyat tavanı düşük.** PiiBlocker 100+ koltukta 4,99 USD. Chrome Enterprise Premium 6 USD. Microsoft 365 Business Premium (~22 USD) içinde keşif var, engelleme için ek lisans gerekiyor ([TMinus365](https://tminus365.com/detecting-shadow-ai-in-your-organization/)). Steward kullanıcı başı 5 USD'nin çok üstüne çıkamaz; fark verim ve rapordan gelmeli.
3. **Verim katmanı en zor ve en abartıya açık parça.** "Haftada ~X saat" tahmini, sadece AI sitelerindeki yapıştırmalardan türetiliyor. Dokümanlar bunu dürüstçe not ediyor. Ama satışta ilk abartı, güveni ve KVKK ölçülülük savunmasını birlikte yakar.
4. **Adaptör kırılganlığı tek geliştiricide ağır.** ChatGPT, Gemini, Copilot arayüzleri sık değişir. Microsoft bile Purview dokümanında ChatGPT'nin "kodlanmış ve dinamik uç noktalar" yüzünden zorlayıcı olduğunu yazıyor. Uzaktan seçici güncelleme şart ama yeterli değil; günlük Playwright testi olmadan ürün sessizce kör olur.
5. **Kapsam dışı yüzey büyük.** Masaüstü uygulamalar, telefon, kişisel bilgisayar, ekran görüntüsü. Rakipler de aynı sorunu yaşıyor; ama Steward'ın "kapsama 34/38" göstergesi gerçekte "tarayıcı kapsamı"dır. Satışta bu dürüstçe söylenmeli.
6. **Guardian Edge Ankara'da, güvenlik firması arkasında.** AltaySec'in LLM pentest, eğitim ve CTF itibarı var. Kurumsal satışta Steward'dan güçlü. KOBİ'de ve verimde ise zayıf.
7. **GB planı dolu bir odaya giriyor.** ChatShield UK hukuk ve muhasebe bürolarına 8–15 GBP'ye satıyor; Harmonic Londra'da; Copilot UK'de 2026 sonunda ülke içi işliyor. "UK regüle meslek şablonu" ayrışma değil.
8. **İsim çakışması.** getsteward.ai bir uyum (compliance) platformu. Steward da "uyum" dili kullanıyor. Aynı kategori, aynı İngilizce konuşan pazar.
9. **Kurucu kası.** Dokümanlar saha ve kanal satışını "yeni bir kas" diye not ediyor. KOBİ'ye tek tek satış yavaş; kanal (IT firması, KVKK danışmanı, SMMM) olmadan ölçek yok.

---

## 4. SWOT

| | **Yardımcı** | **Zararlı** |
| :--- | :--- | :--- |
| **İç** | **Güçlü yönler**<br>• İçerik cihazdan çıkmıyor, doğrulanabilir<br>• Maskele + geri doldur (rakipler engelliyor)<br>• TR veri tipleri + ERP sözlüğü + Türkçe NER<br>• KVKK kanıt raporu<br>• Verim katmanı, kişi değil departman<br>• Düşük sermaye, sıcak pilot | **Zayıf yönler**<br>• Mekanizma kopyalanabilir, artık meta<br>• Tek geliştirici, adaptör bakımı ağır<br>• Verim tahmini abartıya açık<br>• Satış ve kanal kası yok<br>• Tarayıcı dışı kapsam yok<br>• İsim çakışması |
| **Dış** | **Fırsatlar**<br>• KVKK Mart 2026 duyurusu + Eylül 2026 ilke kararı<br>• Copilot TR'de ülke içi işlemiyor, 2028'e kadar liste dışı<br>• Şirketlerde AI kullanımı bir yılda ikiye katlandı (%7,5 → %14)<br>• KVKK danışmanı ve SMMM kanalı<br>• 132 bin ihracatçı KOBİ, orta ölçekte ihracat oranı %31 ([KOSGEB](https://webdosya.kosgeb.gov.tr/Content/Upload/Dosya/Kurumsal/2025/Tu%CC%88rkiye'deki_KOBI%CC%87'lere_I%CC%87lis%CC%A7kin_Baz%C4%B1_I%CC%87statistiki_Go%CC%88stergeler_2025.pdf))<br>• Sıcak satın alma pazarı | **Tehditler**<br>• Chrome Enterprise Premium 6 USD, Edge + Purview paket içinde<br>• ESET 2026 sonunda tarayıcı modülüyle chatbot DLP getiriyor ([Pulse](https://www.pulse.bot/ai/news/eset-previews-new-ai-security-features-to-secure-chatbot-communications-and-ai-workflows-51ba8d94-4da5-4d1a-bb79-f9451527a670/)); KOBİ'lerin AV'si bedava eklenti haline gelirse Steward'ın kalkanı değersizleşir<br>• Guardian Edge TR'de önce kurumsalı alır, sonra aşağı iner<br>• PiiBlocker Türkçe veri tiplerini eklerse 5 USD'lik taban çöker<br>• KVKK denetimi KOBİ'de seyrek; korku yeterince somut olmayabilir<br>• AB AI Act çalışan izleme hükümleri (2027–28) verim katmanını "yüksek risk" sınıfına yaklaştırabilir |

---

## 5. Porter'ın beş gücü (KOBİ gölge AI kalkanı, Türkiye)

| Güç | Şiddet | Neden |
| :--- | :---: | :--- |
| Yeni giriş tehdidi | **Yüksek** | Eklenti yazmak ucuz. PiiBlocker, ChatShield, Guardian Edge 1–2 yılda çıktı. Giriş bariyeri kod değil, dağıtım ve güven. |
| İkame tehdidi | **Yüksek** | Chrome Enterprise Premium (6 USD), Edge + Purview, ESET'in gelecek modülü, ya da basitçe "ChatGPT'yi DNS'ten engelle". KOBİ patronu için "yasak" da bir ikame. |
| Tedarikçi gücü | **Orta** | Chrome Web Store ve Microsoft Edge mağazası tek dağıtım kapısı. Manifest V3 kuralları uzaktan kod yüklemeyi yasaklıyor. AI siteleri arayüzü değiştirince ürün kırılır. |
| Alıcı gücü | **Orta–yüksek** | KOBİ patronu fiyat duyarlı, geçiş maliyeti düşük (eklentiyi kaldır). Ama tek karar verici var ve KVKK korkusu tetiklenirse hızlı alır. |
| Mevcut rekabet | **TR'de düşük, globalde yüksek** | TR'de tek doğrudan rakip Guardian Edge (pilot). Globalde onlarca oyuncu, konsolidasyon hızlı. |

**Okuma:** Sektör yapısı kötü (giriş ve ikame yüksek). Para, yapıdan değil **konumdan** kazanılır: kanal, yerel veri, uyum çıktısı ve verim. Bu, dokümanlardaki "moat'ı koyacağımız yerler" listesiyle örtüşüyor.

---

## 6. Personalar ve işler (Jobs To Be Done)

CLAUDE.md'nin sorusu: "Bu ürün 6 ayda 1 milyar USD değerlemeye ulaşsaydı, kararı kimler verirdi?" Bu dört kişi:

| Persona | Yapmaya çalıştığı iş | Bugün ne yapıyor | Steward'ın satır satır cevabı | Risk |
| :--- | :--- | :--- | :--- | :--- |
| **Patron / GM (Puls)** | "Mühendisim firmware'i ChatGPT'ye yapıştırırsa ilaç müşterim NDA'yı iptal eder. Bunu bilmeden uyuyamam." | Hiçbir şey, ya da sözlü "dikkat edin". | 2 haftalık rapor: "17 kod yapıştırması, 4 fiyat teklifi." Sonra: "Artık maskeleniyor, işte giden metin." | Rapor boş çıkarsa (kimse yapıştırmıyorsa) satış ölür. Faz 0 bunu ölçmeli. |
| **IT sorumlusu** | "Patron 'AI'ı kontrol et' dedi. Bir şey kurup çalışır göstermeliyim, ama çalışanlar bana küfretmesin." | Belki DNS engeli denedi, çalışanlar telefona geçti. | 30 dakikada ERP cari listesi yükle, GPO ile dağıt, kanarya yeşil ışığı gör. | Eklenti kırılırsa suçlu IT olur. Günlük otomatik test şart. |
| **Çalışan / mühendis** | "ChatGPT'yi kullanmaya devam edeyim, kimse beni izlemesin, işim yavaşlamasın." | Kişisel hesapla ChatGPT. | Maskeleme fark edilmez, kişisel görünüm sadece kendisinde, patron kişi görmez. | Yanlış alarm veya bozuk geri doldurma → eklentiyi kapatır. Yanlış alarm oranı ürünün ölçütü. |
| **KVKK danışmanı / SMMM (kanal)** | "Müşterime 'AI politikanız var mı' diye soruyorum, cevap yok. Satacak somut bir şeyim olsun." | Word şablon politika. | Aylık KVKK raporu + politika şablonu + aydınlatma metni. Danışman kanalı, gelir payı. | Danışman kendi "AI danışmanlığını" satmak isteyebilir. Ürün onu rakip değil ortak yapmalı. |

**Çıkarım:** Satın alma kararını patron verir ama korkuyu danışman tetikler. Dokümanlarda kanal olarak sadece IT firmaları var. **KVKK danışmanları ve SMMM ofisleri** ikinci kanal olmalı; raporun ana hipotezindeki "regüle meslek" bu şekilde müşteri değil kanal olur.

---

## 7. Moat analizi (Hamilton Helmer'ın 7 gücü)

| Güç | Steward'da var mı | Not |
| :--- | :---: | :--- |
| Ölçek ekonomisi | Hayır | SaaS marjı herkeste aynı. |
| Ağ etkisi | Zayıf, kurulabilir | ERP sözlüğü ve Türkçe NER her müşteriyle iyileşir (anonim kalıplar). Zor ama gerçek. |
| Karşı konumlanma | **Evet** | Google ve Microsoft "engelle" ile satıyor; "maskele + geri doldur" onların kurumsal DLP modelini bozar. ESET gibi AV'ler içerik kaydetmeye alışkın; "içerik bize gelmez" onlara ters. |
| Geçiş maliyeti | Orta | Sözlük, politika, aylık rapor arşivi birikir. 6 ay sonra bırakmak KVKK kanıt zincirini kırar. |
| Marka | Hayır | Henüz yok; isim çakışması var. |
| Kaynak kilidi | Zayıf | Türk ERP firmalarıyla resmî entegrasyon anlaşması kilit olabilir. |
| Süreç gücü | Orta | Günlük adaptör testi, Türkçe tespit kalitesi, yanlış alarm oranı. Kopyalanabilir ama zaman alır. |

**Okuma:** En güçlü iki kaynak **karşı konumlanma** ve **geçiş maliyeti**. İkisi de kanıt raporu ve sözlüğe dayanıyor, kalkan mekanizmasına değil. Yol haritası bunu doğru görmüş; satış dili de aynı yere gelmeli.

---

## 8. Rekabet haritası (Kasım 2026)

### 8.1 Katman A: Platform sahipleri (asıl tehdit)

| Oyuncu | Ne yapıyor | Fiyat | Maskeleme | Zayıf noktası |
| :--- | :--- | :--- | :---: | :--- |
| **Chrome Enterprise Premium** | AI sitelerine yapıştırma ve yüklemeyi DLP kuralıyla engeller | 6 USD/kullanıcı/ay, satış üzerinden ([Chrome Enterprise](https://chromeenterprise.google/intl/ko/pricing/)) | Hayır | Türkçe veri tipi yok, KVKK raporu yok, sadece engeller. |
| **Microsoft Edge for Business + Purview** | Edge 144+ sürümünde AI uygulamalarına inline DLP: izin ver / engelle / denetle; engellenen istemi Copilot'a yönlendir ([Windows Blog](https://blogs.windows.com/msedgedev/2026/03/23/protect-your-enterprise-from-shadow-AI-and-more-announcements-at-RSAC-2026/)) | Purview lisansı; Business Premium'da keşif var, engelleme için ek lisans ([TMinus365](https://tminus365.com/detecting-shadow-ai-in-your-organization/)) | Hayır | Sadece Edge. Türkiye'deki KOBİ Chrome kullanıyor. Copilot TR'de ülke içi işlemiyor. |
| **ESET (2026 sonu)** | Chatbot istem ve cevaplarını tarayan tarayıcı modülü ([Pulse](https://www.pulse.bot/ai/news/eset-previews-new-ai-security-features-to-secure-chatbot-communications-and-ai-workflows-51ba8d94-4da5-4d1a-bb79-f9451527a670/)) | Mevcut AV paketinde, muhtemelen ek ücretsiz | Belirsiz | Henüz çıkmadı. Türkçe tespit ve KVKK raporu beklenmez. |
| **OpenAI ChatGPT Business** | Eğitimde kullanmama, SSO; kullanım analitiği sadece Enterprise'da ([Gend](https://www.gend.co/blog/chatgpt-for-business)) | 25–30 USD/koltuk | Hayır | Sadece kendi ürünü; gölge kullanım kişisel hesaplarda. |

### 8.2 Katman B: Kurumsal DLP (KOBİ için pahalı)

| Oyuncu | Durum | Fiyat | Not |
| :--- | :--- | :--- | :--- |
| **Harmonic Security** (SF/Londra) | 50M USD Series B, Ekim 2026; 100+ kurumsal müşteri | Açıklanmıyor | Tarayıcı eklentisi + küçük dil modelleri. "Usage Intelligence" verim katmanının kurumsal hâli. En yakın kurumsal benzer. |
| **LayerX** → Akamai | 205M USD, Mayıs 2026 | Açıklanmıyor | Tarayıcı eklentisi. Artık Akamai paketinde. |
| **Prompt Security** → SentinelOne | ~250–300M USD, Ağustos 2025 | Açıklanmıyor | Singularity platformuna entegre. |
| **Nightfall AI** | Tarayıcı DLP | Teklif usulü; 300+ çalışan hedef ([Rhindon](https://raic.rhindoncyber.com/resources/shadow-ai/smb-buyerguide-2026)) | Türkçe yok. |
| **Cyberhaven, Reco, Obsidian** | Kurumsal | 25–40K USD/yıl | KOBİ için erişilmez. |

### 8.3 Katman C: KOBİ ve MSP (fiyat çapası burası)

| Oyuncu | Yaklaşım | Fiyat | Maskele + geri doldur | Admin | Türkçe | KVKK raporu | Verim |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: | :---: |
| **PiiBlocker** | Chrome eklentisi, lokal tespit, 7 AI sitesi | Ücretsiz; Enterprise 6,99 USD (100+ koltukta 4,99) | ✅ Otomatik | ✅ GPO/MDM, metadata raporu | ❌ | ❌ | ❌ |
| **ChatShield** (UK) | Tarayıcı, hukuk ve muhasebe büroları | 8–15 GBP/kullanıcı | ❌ Engeller/işaretler | ✅ Ortak paneli | ❌ | ❌ | ❌ |
| **ShadowLock** | Windows ajanı + yönetilen eklenti, MSP | Cihaz başı, kademeli | Belirsiz | ✅ Çok kiracılı | ❌ | ❌ | ❌ |
| **RAIC** (Rhindon) | Eklenti + M365 sinyali + yönetişim programı | 349 USD/ay'dan | ❌ | ✅ | ❌ | ✅ (NIST, ISO 42001, AI Act) | ❌ |
| **Nudge Security** | E-posta metadata keşfi | 750 USD/ay (<150 kullanıcı) | ❌ | ✅ | ❌ | ❌ | ❌ |
| **DefensX** (ABD, Türk kurucu) | Tarayıcı güvenliği, AI Cloud Connector; 500+ MSP, 7.000+ KOBİ ([Channel Insider](https://www.channelinsider.com/security/tools-and-platforms/defensx-ai-browser-security-msps/)) | MSP üzerinden | Belirsiz | ✅ | ❌ | ❌ | ❌ |
| **Caviard, Private Guard, RedactPII, Privacy Prompt** | Tek kişilik eklentiler | Ücretsiz / tek seferlik | Çoğu ✅ | ❌ | ❌ | ❌ | ❌ |

### 8.4 Katman D: Türkiye

| Oyuncu | Ne yapıyor | Fiyat | Maskele + geri doldur | Türkçe | KVKK | Verim | Zayıf noktası |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: | :--- |
| **AltaySec Guardian Edge** (Ankara) | Chrome eklentisi; ChatGPT, Claude, Gemini; TC, IBAN, kart, telefon, e-posta maskeleme (checksum doğrulamalı); API anahtarı engelleme; kaynak kod uyar/engelle; 3 sözlük; shadow mode; fail-closed ([AltaySec](https://altaysec.com.tr/en/products)) | Yok; pilot programı, 7 gün ücretsiz | ✅ | ✅ 18 TR veri tipi (Guardian) | Dil var, rapor yok | ❌ | İçerik Guardian sunucusunda taranıyor (bulut, TR hosting veya on-prem). Kurumsal güvenlik ekibi hedefi. ERP sözlüğü yok. Copilot adaptörü yok. Verim yok. |
| **kolay.ai, KobiGPT** | AI geçidi ve şirket içi asistan | Açıklanmıyor | Farklı ürün | ✅ | Dil var | ❌ | Gölge AI'ı değil, "resmî AI"ı satıyor. Rakip değil, komşu. |
| **Securefors, NSS, SecureSys** | DLP entegratörü, içerik pazarlaması | Proje | Klasik DLP | – | – | ❌ | Ürün değil, hizmet. |

### 8.5 Katman E: Verim rakipleri

| Oyuncu | Ne yapıyor | Gizlilik | KOBİ'ye uygun mu |
| :--- | :--- | :--- | :---: |
| **Harmonic Usage Intelligence** | Hangi AI kullanımı değer üretiyor | Kurumsal | ❌ |
| **ActivTrak** | "AI workflow intelligence": tekrarlayan işleri bulur, otomasyon fırsatı çıkarır ([Hubstaff](https://hubstaff.com/blog/tools-that-help-monitor-ai-usage-at-work/)) | Çalışan izleme algısı | Orta |
| **Insightful AI Adoption Report** | Ekip bazlı AI aracı kullanımı, olgunluk matrisi; sadece metadata ([Insightful](https://www.insightful.io/ai-adoption)) | Metadata-only, ekip düzeyi | Orta |
| **Worklytics** | Copilot/Gemini bağlantılı, anonim, departman kalıpları | Anonim | ❌ (kurumsal) |

**Okuma:** Verimde en yakın benzer Insightful: metadata-only, ekip düzeyi, gizlilik vurgusu. Ama Insightful masaüstü ajanıyla tüm uygulamaları sayıyor ve "zaman tasarrufu" iddiası yapmıyor. Steward'ın "görev türü sınıflandırma + tek tuşla şablon" fikri hâlâ boş. ActivTrak otomasyon fırsatı çıkarıyor ama gözetleme aracı olarak algılanıyor; 2026/2035 kararı onu Türkiye'de zorlar.

### 8.6 Güncellenmiş konum haritası

```
                 Engelle / denetle            Maskele + geri doldur
               ┌──────────────────────────┬──────────────────────────┐
  Kurumsal     │ Purview, Chrome Premium  │ Harmonic, LayerX/Akamai, │
  (250+)       │ Nightfall, Cyberhaven    │ Prompt/SentinelOne       │
               ├──────────────────────────┼──────────────────────────┤
  KOBİ         │ ChatShield (UK), RAIC,   │ PiiBlocker, ShadowLock?, │
  (10–250)     │ Nudge, DefensX           │ Guardian Edge (TR) ★     │
               │                          │ ► STEWARD: + ERP sözlüğü │
               │                          │   + KVKK raporu + verim  │
               ├──────────────────────────┼──────────────────────────┤
  Birey        │ DNS engeli               │ Caviard, Private Guard,  │
               │                          │ RedactPII, Perplexity    │
               └──────────────────────────┴──────────────────────────┘
```

Sağ-orta hücre artık boş değil. Steward'ın farkı hücrenin içinde değil, hücreye eklediği üç şeyde.

---

## 9. Pazar büyüklüğü (Türkiye)

| Gösterge | Değer | Kaynak |
| :--- | :--- | :--- |
| Aktif girişim (2025) | 4.016.059 | [Forbes TR / TÜİK](https://www.forbes.com.tr/ekonomi/sanayi-ve-hizmet-sektorunun-2025-yili-karnesi-belli-oldu) |
| KOBİ (2023) | ~3,71 milyon, %99,7 | [KOSGEB](https://webdosya.kosgeb.gov.tr/Content/Upload/Dosya/Kurumsal/2025/Tu%CC%88rkiye'deki_KOBI%CC%87'lere_I%CC%87lis%CC%A7kin_Baz%C4%B1_I%CC%87statistiki_Go%CC%88stergeler_2025.pdf) |
| İstihdam payı 10–49 / 50–249 | %19,6 / %17,0 | Forbes TR / TÜİK |
| İhracatçı KOBİ (2023) | ~132.000; orta ölçekte ihracat oranı %31,3 | KOSGEB |
| Şirketlerde AI kullanımı (2026) | 10–49: %12,8; 50–249: %17,0 | [TÜİK via Quasa](https://quasa.io/tr/media/turkiyede-sirketlerin-ai-kullanimi-ikiye-katlandi-insaat-yuzde-69da-kaldi) |
| Bireylerde üretken AI (2026) | %37,6 (2025: %19,2) | TÜİK |

**Tahmin (doğrulanmalı):** TÜİK'in önceki yıl dağılımlarına göre Türkiye'de 10–49 çalışanlı yaklaşık 200 bin, 50–249 çalışanlı yaklaşık 40 bin girişim var. Bu sayılar KOSGEB raporunun Tablo 3'ünden kesinleştirilmeli.

**Hedef daraltma:**
- SAM: 50–249 çalışan + ihracatçı veya regüle (ilaç/gıda tedarikçisi, SMMM, hukuk, klinik) ≈ 15–20 bin şirket.
- SOM (24 ay): 200 şirket × ortalama 40 kullanıcı × 5 USD × 12 ay ≈ **480 bin USD ARR**. Bu bir YC ölçeği değil, ama tek kurucu için sağlıklı bir işletme ve kanal ortağıyla 5–10 kat büyür.

**Fiyat önerisi (tartışmaya açık):** Kullanıcı başı değil, **şirket başı kademeli sabit** (ör. 10'a kadar, 50'ye kadar, 250'ye kadar). Gerekçe: patron şirket için öder, koltuk saymaz; IT koltuk kısmaz; PiiBlocker'ın 4,99 USD çapasıyla doğrudan kıyaslanmaz; KVKK raporu şirket düzeyinde bir ürün.

---

## 10. Pre-mortem: Steward 12 ay sonra neden ölmüş olabilir?

1. **Faz 0 raporu boş çıktı.** Puls'ta 2 haftada 3 yapıştırma yakalandı, patron "sorun yokmuş" dedi. → Faz 0'a kanarya dışında "en az 5 cihaz ve mühendis" şartı koy; sonuç boşsa segmenti değiştir, ürünü değil.
2. **Eklenti iki kez kırıldı, IT sorumlusu kaldırdı.** → Günlük Playwright adaptör testi Faz 0'da olmalı, Faz 1'de değil.
3. **Verim raporu abartı çıktı, patron güvenini kaybetti.** → Faz 0 ve 1'de saat tahmini verme; sadece "haftada ~40 çeviri isteği" gibi sayım ver. Saat tahmini ancak müşteri onaylı bir şablon kullanıldıktan sonra, ölçülen veriden.
4. **ESET veya Chrome bedava kalkan getirdi, kalkan fiyatı sıfıra indi.** → Gelirin yarısı 12 ay içinde rapor + verim + sözlükten gelmeli. Kalkan tek başına fiyatlanmamalı.
5. **Guardian Edge KOBİ'ye indi, kurumsal referanslarıyla kazandı.** → Steward'ın cevabı "içerik hiç çıkmaz" + ERP sözlüğü + 30 dakikada kurulum. Bunu ilk günden ölçülebilir kıyas tablosu olarak yayınla.
6. **Tek tek satış, ayda 1 müşteri.** → 3. müşteriden sonra kanal: 2 IT firması + 2 KVKK danışmanı, gelir payı.
7. **GB'ye Steward adıyla gidildi, getsteward.ai itiraz etti.** → GB fazından önce ayrı marka veya TR'de kalma kararı.

---

## 11. Skor kartı güncellemesi

Pazar araştırması dokümanı on-prem fikri için 22/40 vermişti. Gölge AI kalkanı + verim konumu için:

| Faktör | Eski | Yeni | Gerekçe |
| :--- | :---: | :---: | :--- |
| Acının gerçekliği | 4 | **4** | KVKK duyurusu ve ilke kararı; Copilot TR dışı kaldı. |
| Ödeme isteği (KOBİ) | 2 | **3** | Verim katmanı ve ceza çapası artırıyor; saha doğrulaması hâlâ sıfır. |
| Türkiye'de rekabet boşluğu | 4 | **3** | Guardian Edge var. Boşluk ürün değil, konum (KOBİ + rapor + verim). |
| Global rekabet boşluğu | 2 | **1** | PiiBlocker, ChatShield, Harmonic, Akamai. GB planı dolu. |
| Teknik risk | 3 | **4** | Donanım yok, hibrit mimari doğrulandı. Risk adaptör bakımına indi. |
| Donanım/operasyon riski | 2 | **4** | Yazılım-öncelikli, kutu Faz 2'ye ertelendi. |
| Moat | 2 | **3** | Karşı konumlanma + geçiş maliyeti; ERP sözlüğü, KVKK kanıt zinciri. |
| Kurucu uyumu | 3 | **4** | Sıcak pilot, eklenti ve panel tek geliştiricinin alanında; kanal hâlâ açık. |
| **Toplam** | **22/40** | **26/40** | |

---

## 12. Tartışılacak kararlar

1. **Konumlandırma:** "Gölge AI kalkanı" mı, "KVKK kanıtı + AI verim haritası" mı? Öneri: ikincisi. Kalkan ürünün içinde kalır, başlıkta değil.
2. **Fiyat modeli:** Kullanıcı başı (PiiBlocker çapası 5 USD) mi, şirket başı kademeli sabit mi? Öneri: şirket başı.
3. **Guardian Edge'e karşı dil:** "İçerik sunucuya hiç gelmez" + ERP sözlüğü + 30 dakikada kurulum. Pilot teklifinde AltaySec kıyası açıkça verilsin mi?
4. **Verim katmanında abartı sınırı:** Faz 0 ve 1'de saat tahmini verilmesin, sadece sayım. Faz 1.1'de ölçülen veriyle saat. Kabul mü?
5. **Kanal:** IT firmalarına ek olarak KVKK danışmanları ve SMMM ofisleri. Regüle meslekler müşteri değil kanal. Puls'tan sonraki ilk 2 görüşme danışmanla mı olsun?
6. **GB fazı:** ChatShield, Harmonic ve Copilot UK gerçeğiyle GB planı yeniden yazılmalı. Şimdilik "TR'de 10 ücretli müşteri" eşiği kalsın, GB için ayrı marka araştırılsın mı?
7. **İsim:** Steward çalışma adı olarak kalsın; TÜRKPATENT sorgusu bu hafta; GB için alternatif liste çıkarılsın mı?
8. **Faz 0'a ek:** Günlük Playwright adaptör testi ve "en az 5 cihaz, 1 mühendis" şartı Faz 0'a taşınsın mı?

---

## 13. Kaynaklar

- KVKK duyurusu: [ACR Legal](https://ayseeceacar.av.tr/kvkk-uyardi-is-yerinde-golge-yapay-zeka-kullanmak-artik-risk-cursor-ve-kimi-davasi-ne-gosteriyor/), [Anka Law](https://www.anka.law/makaleler/kisisel-verileri-koruma-kurumunun-yeni-dokumani-isiginda-golge-yapay-zeka/), [Erdem & Erdem](https://www.erdem-erdem.av.tr/bilgi-bankasi/is-yerlerinde-uretken-yapay-zeka-araclarinin-kullanimi-baslikli-kisisel-verileri-koruma-kurumu-duyurusu-yayimlandi)
- KVKK ilke kararı 2026/2035: [Erdem & Erdem](https://www.erdem-erdem.av.tr/bilgi-bankasi/kurumsal-iletisim-araclarinin-denetlenmesine-iliskin-ilke-karari-yayimlandi), [Forbes TR](https://www.forbes.com.tr/haberler/isverenler-artik-calisanlarin-e-postalarini-gizlice-denetleyemeyecek), [Alomaliye](https://www.alomaliye.com/2026/10/08/isverenin-e-posta-denetimine-sinir/)
- KVKK 2026 cezaları: [CottGroup](https://cottgroup.com/tr/mevzuat/item/yeniden-degerleme-oranina-gore-2026-yili-kvkk-idari-para-cezalari)
- TÜİK 2026 AI kullanımı: [Quasa](https://quasa.io/tr/media/turkiyede-sirketlerin-ai-kullanimi-ikiye-katlandi-insaat-yuzde-69da-kaldi), [Milliyet / Mahmut Özer](https://www.milliyet.com.tr/yazarlar/prof-dr-mahmut-ozer/tuik-yapay-zeka-2026-yili-istatistikleri-ne-soyluyor-7672996)
- TÜİK 2025 girişim istatistikleri: [Forbes TR](https://www.forbes.com.tr/ekonomi/sanayi-ve-hizmet-sektorunun-2025-yili-karnesi-belli-oldu); KOBİ göstergeleri: [KOSGEB 2025](https://webdosya.kosgeb.gov.tr/Content/Upload/Dosya/Kurumsal/2025/Tu%CC%88rkiye'deki_KOBI%CC%87'lere_I%CC%87lis%CC%A7kin_Baz%C4%B1_I%CC%87statistiki_Go%CC%88stergeler_2025.pdf)
- Microsoft Copilot ülke içi işleme: [Microsoft](https://www.microsoft.com/en-us/microsoft-365/blog/2025/11/04/microsoft-offers-in-country-data-processing-to-15-countries-to-strengthen-sovereign-controls-for-microsoft-365-copilot/)
- Edge + Purview: [Windows Blog RSAC 2026](https://blogs.windows.com/msedgedev/2026/03/23/protect-your-enterprise-from-shadow-AI-and-more-announcements-at-RSAC-2026/), [Microsoft Learn](https://learn.microsoft.com/en-us/purview/dlp-browser-dlp-learn), [TMinus365](https://tminus365.com/detecting-shadow-ai-in-your-organization/), [Aona](https://aona.ai/blog/microsoft-edge-shadow-ai-controls-not-enough/)
- Chrome Enterprise Premium: [fiyat](https://chromeenterprise.google/intl/ko/pricing/)
- Guardian Edge: [ürün sayfası](https://altaysec.com.tr/urunler/guardian-edge), [ürünler](https://altaysec.com.tr/en/products)
- PiiBlocker: [site](https://www.piiblock.com/), [eklenti karşılaştırması](https://www.piiblock.com/blog/best-pii-masking-chrome-extensions-ai-chatbots)
- ChatShield: [Capterra](https://www.capterra.com/p/10044878/ChatShield/)
- KOBİ alıcı rehberi (RAIC, Nudge, Nightfall, Cyberhaven, Reco, Obsidian, Lavawall): [Rhindon](https://raic.rhindoncyber.com/resources/shadow-ai/smb-buyerguide-2026), [Nudge Security](https://www.nudgesecurity.com/post/best-shadow-ai-detection-tools), [ShadowLock](https://shadowlock.io/blog/best-ai-dlp-tools/)
- Harmonic Series B: [Unite.AI](https://unite.ai/harmonic-security-raises-50m-series-b-to-expand-us-and-uk-teams)
- Akamai–LayerX: [haber](https://the-coders-blog.pages.dev/akamai-buys-layerx-a-205m-bet-on-ai-browser-security/)
- SentinelOne–Prompt Security: [SiliconANGLE](https://siliconangle.com/2025/08/05/sentinelone-acquires-ai-security-startup-prompt-security/)
- Check Point–Lakera: [SecurityWeek](https://www.securityweek.com/check-point-to-acquire-ai-security-firm-lakera/)
- DefensX: [Channel Insider](https://www.channelinsider.com/security/tools-and-platforms/defensx-ai-browser-security-msps/)
- ESET AI güvenlik önizlemesi: [Pulse](https://www.pulse.bot/ai/news/eset-previews-new-ai-security-features-to-secure-chatbot-communications-and-ai-workflows-51ba8d94-4da5-4d1a-bb79-f9451527a670/)
- Verim araçları: [Hubstaff karşılaştırması](https://hubstaff.com/blog/tools-that-help-monitor-ai-usage-at-work/), [Insightful](https://www.insightful.io/ai-adoption)
- ChatGPT Business fiyatı: [Gend](https://www.gend.co/blog/chatgpt-for-business)
- Perplexity Hybrid Compute: [Unite.AI](https://www.unite.ai/perplexity-launches-hybrid-compute-on-mac-with-local-privacy-gate/)
- Steward (AML) isim çakışması: [tech.eu](https://tech.eu/2026/03/17/steward-an-ai-driven-compliance-platform-managing-100b-raises-5m/)
- Türkçe NER modelleri (tarayıcıda çalıştırma için aday): [akdeniz27 quantized](https://huggingface.co/akdeniz27/convbert-base-turkish-cased-ner-quantized), [girayyagmur](https://huggingface.co/girayyagmur/bert-base-turkish-ner-cased)
