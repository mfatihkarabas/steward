# Rakip Araştırması: Global ve Yerel, Okyanus Rengi ve Referans Sıralaması

**Tarih:** 2026-11-07
**Bu dosyanın rolü:** `2026-11-06-FikirAnalizi.md` bölüm 8'deki rekabet haritasını derinleştirir. Her rakibi yatırım, ticari çekiş ve memnuniyet verisiyle puanlar, güçlüden zayıfa sıralar, geliştirme sürecinde kimden ne öğrenileceğini söyler ve "kırmızı mı mavi mi" sorusunu cevaplar.
**Veri notu:** Yatırım ve müşteri sayıları haber ve şirket açıklamalarından; memnuniyet G2 ve Gartner Peer Insights puanlarından. Yorum sütunu benim değerlendirmem. Türk şirketlerinin çoğu yatırım ve müşteri açıklamıyor; bunlar "açıklanmadı" olarak işaretli.

---

## 0. Özet

- **Global kurumsal pazar kırmızı.** Gartner 2026'da "AI Usage Control" diye ayrı bir kategori açtı ve 20 satıcı listeliyor. 14 ayda beş satın alma oldu (Prompt Security, Lakera, Aim, LayerX, Fiddler/Dreadnode). Island 6,4 milyar USD değerlemeye çıktı. Bu rafa yeni girilmez.
- **Global KOBİ rafı sığ mavi.** Ucuz eklentiler var ama çekişleri yok: PiiBlocker'ın Chrome mağazasında 521 kullanıcısı var. "Sadece kalkan" ürünlerine KOBİ para vermiyor. Nudge Security (200 müşteri, 2 yıl üst üste 3 kat ARR) KOBİ'de işleyen tek modeli gösteriyor: sabit aylık fiyat, davranış dürtme, engelleme değil.
- **Türkiye KOBİ rafı mavi ama boş değil.** AltaySec Guardian Edge (pilot), SHIM (Product Hunt, Ocak 2026, 3 oy), kolay.ai (kurumsal geçit), ALP DLP (klasik DLP) var. Hiçbirinin açıklanmış ücretli KOBİ müşterisi yok. Pazar yaratılmayı bekliyor; bu hem fırsat hem uyarı.
- **Karar:** The Great Project mavi okyanusu "kalkan" ile değil, Mavi Okyanus'un ERRC çerçevesiyle **yaratır**: içerik bulutunu ve koltuk fiyatını kaldır, kurumsal karmaşıklığı azalt, yerel tespit ve doğrulanabilirliği yükselt, KVKK kanıtı, ERP sözlüğü ve verim haritasını yarat (bölüm 6).
- **İlk beş referans:** Harmonic (konum ve verim katmanı), LayerX (eklenti kalitesi ve memnuniyet), Nudge (KOBİ fiyat ve dürtme modeli), Strac (10 dakikada kurulum çıtası), Guardian Edge (yerel rakibin tespit seti). Bölüm 7'de kimden ne alınacağı var.

---

## 1. Puanlama yöntemi

Dört ölçüt, her biri 1–5:

| Ölçüt | Ne ölçer | Veri |
| :--- | :--- | :--- |
| **Y** Yatırım ve çıkış | Toplam yatırım, değerleme, satın alma | Haberler |
| **Ç** Ticari çekiş | Müşteri, ARR, kullanıcı, büyüme | Şirket açıklamaları |
| **M** Memnuniyet | G2 / Gartner Peer Insights puanı ve yorum sayısı; veri yoksa ürün sayfasından benim değerlendirmem (★ ile işaretli) | G2, Gartner |
| **R** The Great Project'e referans değeri | Yaklaşım benzerliği (eklenti, maskele + geri doldur, KOBİ, verim) ve öğrenilebilirlik | Benim değerlendirmem |

Toplam 20 üzerinden. Sıralama toplam puana göre; eşitlikte R öne alınır.

---

## 2. Global sıralama (güçlüden zayıfa)

| # | Rakip | Yaklaşım | Yatırım / çıkış | Çekiş | Memnuniyet | Y | Ç | M | R | **Top** |
| :-: | :--- | :--- | :--- | :--- | :--- | :-: | :-: | :-: | :-: | :-: |
| 1 | **Harmonic Security** (SF/Londra) | Tarayıcı eklentisi + uç noktada küçük dil modelleri; "Usage Intelligence" | 76M USD toplam; 50M Series B Ekim 2026 ([Unite.AI](https://unite.ai/harmonic-security-raises-50m-series-b-to-expand-us-and-uk-teams)) | 100+ kurumsal müşteri, milyonlarca çalışan | G2 4,6 (6 yorum); Gartner 5,0 (1) | 4 | 3 | 4 | 5 | **16** |
| 2 | **LayerX** → Akamai Workforce Protector | Tarayıcı eklentisi (Chrome, Edge, Safari, Firefox) | 205M USD nakit, Mayıs 2026; 2026 sonu ~10M USD ARR beklentisi ([haber](https://the-coders-blog.pages.dev/akamai-buys-layerx-a-205m-bet-on-ai-browser-security/)) | Orta; Akamai kanalına giriyor | G2 4,9 (31); Gartner 4,6 (23) ([G2](https://www.g2.com/products/layerx-browser-security-platform/reviews), [Gartner](https://www.gartner.com/reviews/market/ai-usage-control)) | 4 | 3 | 5 | 4 | **16** |
| 3 | **Island** | Kurumsal tarayıcı (Chromium çatalı), DLP + SASE | 400M USD Series F, 6,4 milyar USD değerleme, Eylül 2026 ([FF News](https://ffnews.com/news/island-announces-400-million-series-f-bringing-valuation-to-6-4-billion-8ad14d83)) | ARR her yıl ikiye katlanıyor | Gartner güçlü (kurumsal tarayıcı pazarı) ★4 | 5 | 5 | 4 | 2 | **16** |
| 4 | **Cyberhaven** | Uç nokta ajanı, veri soyağacı (lineage) | 100M USD Series D, 1 milyar USD değerleme, Nisan 2025; 250M toplam ([Techleap](https://finder.techleap.nl/news/feed/cyberhaven-raises-100m-hits-1b-valuation)) | Kurumsal; 36–40K USD/yıl giriş | G2 4,5 (19) | 5 | 4 | 4 | 2 | **15** |
| 5 | **Nightfall AI** | Tarayıcı DLP + SaaS API; yanlış alarm yönetimi öne çıkıyor | ~60M USD toplam (40M Series B) | Oscar Health, Splunk, Exabeam; 300+ çalışan hedef | G2 4,6 (101) ([G2](https://www.g2.com/products/nightfall-ai/reviews)) | 3 | 4 | 4 | 4 | **15** |
| 6 | **Nudge Security** (Austin) | E-posta metadata keşfi + tarayıcı ve Slack'te "dürtme" | 22,5M USD Series A, Kasım 2025 ([Nudge](https://www.nudgesecurity.com/press/nudge-security-raises-22-5m-series-a-to-secure-workforce-ai-and-saas)) | ~200 müşteri; 2 yıl üst üste 3 kat ARR; 750 USD/ay sabit (<150 kullanıcı) | ★4 (G2 verisi alınmadı; KOBİ alıcı rehberlerinde olumlu) | 3 | 3 | 4 | 4 | **14** |
| 7 | **Prompt Security** → SentinelOne | Tarayıcı eklentisi + AI uygulama güvenliği | ~250–300M USD, Ağustos 2025 ([SiliconANGLE](https://siliconangle.com/2025/08/05/sentinelone-acquires-ai-security-startup-prompt-security/)) | SentinelOne Singularity içinde | Gartner 4,2 (14) | 4 | 3 | 3 | 4 | **14** |
| 8 | **Strac** | SaaS + tarayıcı DLP; AI'a gitmeden redaksiyon, kasaya yazma; 10 dakikada ajan­sız kurulum | Küçük (açıklanmadı) | Agentnoon ve küçük SaaS'lar | G2 4,9 (31) ([G2](https://www.g2.com/products/strac/reviews)) | 2 | 2 | 5 | 4 | **13** |
| 9 | **WitnessAI** | Kurumsal AI güvenlik ve yönetişim; ajan güvenliği | 58M USD Ocak 2026 + 27,5M Series A ([Pulse2](https://pulse2.com/witnessai-58-million-raised-to-expand-globally-and-roll-out-new-security-controls-for-ai-agents)) | ARR +%500/yıl; büyük halka açık şirketler | Gartner 4,0 (4) | 4 | 3 | 3 | 2 | **12** |
| 10 | **Metomic** (Londra) | SaaS veri güvenliği, AI araçlarına veri akışı izleme | ~25M USD toplam, 20M Series A ([SecurityWeek](https://www.securityweek.com/metomic-lands-20-series-a-for-data-security-platform/)) | Revolut, Oyster, Juni; müşterilerin yarısı ABD | ★3 | 3 | 3 | 3 | 2 | **11** |
| 11 | **Aim Security** → Cato Networks | Çalışan AI kullanımı + özel AI uygulama güvenliği | 28M USD yatırım; satın alma Eylül 2025, bedel açıklanmadı ([SecurityWeek](https://www.securityweek.com/cato-networks-acquires-ai-security-firm-aim-security/)) | Cato SASE içinde (300M+ USD ARR) | ★3 | 3 | 2 | 3 | 3 | **11** |
| 12 | **Lasso Security** | Ajan ve LLM uygulama guardrail (CPU, <5 ms) | 37M USD toplam, 30M Eylül 2026 ([AI Weekly](https://aiweekly.co/alerts/lasso-security-raises-30m-ships-leap-cpu-only-guardrail-with-sub-5ms-verdicts)) | Gelir +%500 | Gartner 3,5 (2) | 3 | 3 | 2 | 2 | **10** |
| 13 | **Knostic** | Copilot'ta aşırı paylaşımı önleyen erişim kontrolü | ~19M USD ([Virginia Business](https://virginiabusiness.com/knostic-raises-16m-to-secure-generative-ai-data)) | Açıklanmadı | ★3 | 3 | 2 | 3 | 1 | **9** |
| 14 | **Lakera** → Check Point | Uygulama tarafı guardrail, prompt injection | ~300M USD, Eylül 2025 ([SecurityWeek](https://www.securityweek.com/check-point-to-acquire-ai-security-firm-lakera/)) | Check Point içinde | ★3 | 4 | 3 | 3 | 1 | **11** |

**Yardımcı referanslar (rakip değil, parça tedarikçisi):**

| Oyuncu | Ne | Veri | The Great Project'e değeri |
| :--- | :--- | :--- | :--- |
| **Microsoft Presidio** | Açık kaynak PII tanıma ve anonimleştirme çatısı | Microsoft çok yıllı ölçekleme anlaşması ([hoop.dev](https://hoop.dev/blog/microsoft-signs-multi-year-deal-to-scale-presidio-data-protection-framework)) | Tespit kütüphanesinin mimarisi (tanıyıcı + doğrulayıcı + anonimleştirici) buradan alınır |
| **Private AI** (Toronto) | PII redaksiyon API'si, "yazılım için gizlilik katmanı" | 8M + 3,15M USD ([Private AI](https://private-ai.com/?p=8547)) | Tespit kalitesi için kıyas noktası |
| **Ollama** | Lokal model çalıştırma | 88M USD toplam, 65M Series B Temmuz 2026; 8,9M aylık aktif geliştirici ([Noqta](https://noqta.tn/en/news/ollama-65m-series-b-local-ai-open-source-2026)) | Faz 2 kutunun motoru; lokal AI'ın ana akım olduğunun kanıtı |
| **Open WebUI** | Lokal sohbet arayüzü | 149K GitHub yıldızı, BSD-3 ([IdeaProof](https://ideaproof.io/open-source/project/open-webui)) | Faz 2 kutu arayüzü; "bedava alternatif" fiyat çapası |
| **Perplexity Hybrid Compute** | Mac'te lokal maskeleme + bulut akıl yürütme | Ürün içi, Eylül 2026 | Maskele + geri doldur UX'inin tüketici kanıtı |

---

## 3. KOBİ ve MSP rafı (güçlüden zayıfa)

| # | Rakip | Yaklaşım | Fiyat | Çekiş | Memnuniyet | Y | Ç | M | R | **Top** |
| :-: | :--- | :--- | :--- | :--- | :--- | :-: | :-: | :-: | :-: | :-: |
| 1 | **Nudge Security** | Yukarıda; KOBİ'de tek kanıtlı model | 750 USD/ay sabit | 200 müşteri, 3x ARR | ★4 | 3 | 3 | 4 | 4 | **14** |
| 2 | **DefensX** (ABD, Türk kurucu Halis Osman Erkan) | Tarayıcı güvenliği + AI Cloud Connector, MSP kanalı | MSP üzerinden | 500+ MSP, 7.000+ KOBİ ([Channel Insider](https://www.channelinsider.com/security/tools-and-platforms/defensx-ai-browser-security-msps/)) | ★3 | 3 | 4 | 3 | 4 | **14** |
| 3 | **Strac** | Yukarıda | Açıklanmadı | Küçük | G2 4,9 (31) | 2 | 2 | 5 | 4 | **13** |
| 4 | **RAIC** (Rhindon Cyber) | Eklenti + M365 sinyali + yönetişim programı; çok kiracılı | 349 USD/ay'dan ([Rhindon](https://raic.rhindoncyber.com/resources/shadow-ai/smb-buyerguide-2026)) | Açıklanmadı | ★3 | 1 | 2 | 3 | 4 | **10** |
| 5 | **ShadowLock** | Windows ajanı + yönetilen eklenti; redaksiyon, allow/warn/block, kişisel hesap tespiti | 1 USD/cihaz/ay'dan ([Capterra](https://www.capterra.com/p/10048807/ShadowLock/)) | Açıklanmadı | ★3 | 1 | 2 | 3 | 4 | **10** |
| 6 | **ChatShield** (UK) | Tarayıcı; hukuk ve muhasebe büroları; engelle/işaretle | 8–15 GBP/kullanıcı ([Capterra](https://www.capterra.com/p/10044878/ChatShield/)) | Açıklanmadı | ★3 | 1 | 2 | 3 | 3 | **9** |
| 7 | **PiiBlocker** | Chrome eklentisi, lokal maskele + geri doldur, admin paneli, GPO | Ücretsiz; 4,99–6,99 USD/koltuk | **521 kullanıcı** Chrome mağazasında ([Chromeboard](https://chromeboard.com/extension/piiblocker-mask-pii-in-ai-nklghhkmhkmckonncilnaohlihfacoee)) | ★3 | 1 | 1 | 3 | 4 | **9** |
| 8 | Private Guard, Caviard, RedactPII, PromptMask | Tek kişilik eklentiler | Ücretsiz | Private Guard 14 kullanıcı ([Chromeboard](https://chromeboard.com/extension/private-guard-—-pii-redac-jjkghegjofelkblppppihfacdoemjban)) | ★2 | 1 | 1 | 2 | 2 | **6** |

**Okuma:** Bu rafta kazanan yok. En güçlü ikisi (Nudge, DefensX) maskeleme ürünü değil; biri keşif + dürtme, öteki MSP kanalı. Maskeleme eklentilerinin kullanıcı sayısı yüzlerle ölçülüyor. Bu, iki şeyi aynı anda söyler: **(a)** "sadece kalkan" ürünü için talep kanıtlanmamış, **(b)** kanalsız bir eklenti, ne kadar iyi olursa olsun, dağıtılmıyor. The Great Project'in kanıt + verim + kanal vurgusu bu veriyle doğrulanıyor.

---

## 4. Verim katmanı referansları

| Oyuncu | Veri | The Great Project'e değeri |
| :--- | :--- | :--- |
| **ActivTrak** | 1M+ kullanıcı, 9.500+ kurum, gelir +%26, kurumsal ARR +%47 (2025); Francisco Partners yatırımı; 2026'da "AI Workflow Intelligence: tekrarlayan işleri sınıflandırıp otomasyon fırsatı çıkarır" ([ActivTrak](https://www.activtrak.com/news/press-release-momentum-2026/)) | Patrona "AI benimseme ve etki" raporunun nasıl sunulduğu. Ama uç nokta ajanı ve kişi bazlı izleme; KVKK 2026/2035 kararıyla TR'de zor. The Great Project aynı çıktıyı departman düzeyinde, içerik görmeden verir |
| **Harmonic Usage Intelligence** | Hangi AI kullanım senaryosu değer üretiyor | Kurumsal tarafta "verim katmanı"nın var olduğunun kanıtı; KOBİ için yok |
| **Insightful AI Adoption Report** | Ekip bazlı AI aracı kullanımı, olgunluk matrisi; sadece metadata; zaman tasarrufu iddiası yok ([Insightful](https://www.insightful.io/ai-adoption)) | Verim raporunda **ne iddia edilmeyeceği**nin örneği; Faz 0–1 "sadece sayım" kararıyla uyumlu |
| **Worklytics** | Copilot/Gemini bağlantılı, anonim, departman kalıpları | Departman düzeyi anonimleştirme yaklaşımı |

---

## 5. Türkiye (güçlüden zayıfa)

| # | Oyuncu | Yaklaşım | Yatırım | Çekiş | Durum | The Great Project'e göre | **Top** |
| :-: | :--- | :--- | :--- | :--- | :--- | :--- | :-: |
| 1 | **AltaySec Guardian Edge** (Ankara, 2025) | Chrome eklentisi; ChatGPT, Claude, Gemini; 18 TR veri tipi checksum'lu; sözlük; shadow mode; fail-closed; geri doldurma; Guardian geçidi on-prem ([AltaySec](https://altaysec.com.tr/en/products)) | Açıklanmadı | Açıklanmadı; pilot programı, 7 gün ücretsiz | Pilot. Şirketin asıl işi LLM pentest ve eğitim; CTF itibarı var | İçeriği sunucuda tarıyor; kurumsal güvenlik ekibi hedefi; ERP sözlüğü, KVKK raporu, verim, Copilot adaptörü yok | **10** |
| 2 | **kolay.ai** (Levent, İstanbul) | Kurumsal AI geçidi: çok sağlayıcı, politika, maskeleme kuralı, on-prem/VPC, TL fatura ([kolay.ai](https://kolay.ai/)) | Açıklanmadı | Açıklanmadı | Canlı | Gölge AI'ı görmez; "resmî AI" satar; kurumsal | **9** |
| 3 | **SHIM** (getshim.tech) | Geçit: maskeleme + denetim katmanı, TR ve EN veri, self-host veya bulut, shim-cli; **SHIM Shield** adlı tarayıcı eklentisi geliştiriliyor ([Product Hunt](https://www.producthunt.com/products/shim/launches), [Dev.to](https://dev.to/businnect/how-to-secure-ai-applications-without-slowing-them-down-inside-shims-privacy-first-ai-gateway-4aia)) | Workup 14. dönem | Product Hunt 19 Ocak 2026, 3 oy | Geliştirme | The Great Project'e en çok benzeyen TR girişimi, ama geliştirici ve fintech odaklı. Eklentisi çıkarsa doğrudan rakip | **7** |
| 4 | **ALP DLP** (Teknopark İstanbul, Cube) | Klasik uç nokta DLP: USB, yazıcı, pano, web, e-posta; OCR ve AI asistan geliştiriliyor; "AI kullanım yönetişimi"ne genişleme planı ([İTG](https://istanbulticaretgazetesi.com/fikir-okul-sohbetinde-cikti-simdi-veri-sizintisina-set-cekiyor)) | Kuluçka; yatırım yok | Referans arıyor | Erken | Farklı kategori; ileride AI kullanım kontrolü ekleyebilir | **6** |
| 5 | **KobiGPT** (X Mind) | Şirket içi veriyle asistan, on-prem opsiyonu | Açıklanmadı | Açıklanmadı | Canlı | Komşu ürün; kalkan değil | **5** |
| – | Picus, Logsign, Roksit, Crypttech | Klasik siber güvenlik; AI/ML bileşenli ([AltaySec listesi](https://altaysec.com.tr/arastirmalar/turkiye-yapay-zeka-guvenligi-sirketleri-2026)) | Picus büyük | Kurumsal | – | Rakip değil; olası kanal ortağı (özellikle Roksit DNS güvenliği KOBİ'de yaygın) | – |

**Okuma:** Türkiye'de üç oyuncu aynı yöne bakıyor ama üçü de kurumsal veya geliştirici kapısından giriyor. KOBİ patronuna, IT firması kanalıyla, sabit fiyatla, KVKK raporu ve verim haritasıyla giden kimse yok. SHIM'in "SHIM Shield" eklentisi izlenmeli; en hızlı kapanabilecek boşluk bu.

---

## 6. Kırmızı mı, mavi mi?

### 6.1 Dört hücre

| | Kurumsal (250+) | KOBİ (10–250) |
| :--- | :--- | :--- |
| **Global** | 🔴 **Kırmızı.** Gartner AIUC kategorisinde 20 satıcı; 14 ayda 5 satın alma; Island 6,4 milyar USD; Netskope'a göre iç kullanıcıların genAI'a gönderdiği veri bir yılda 30 kat arttı ([Sacra](https://sacra.com/chat/h/265c3bc4-bd8f-4830-b92f-91ead5e35a2e/)) | 🟣 **Sığ mavi.** Ucuz eklentiler yüzlerce kullanıcıda; Nudge ve DefensX kanıtlı ama maskeleme yapmıyor; ChatShield UK niş |
| **Türkiye** | 🟠 **Turuncu.** Guardian Edge ve kolay.ai kurumsalı hedefliyor; kazanan yok | 🔵 **Mavi.** Ücretli KOBİ müşterisi açıklayan kimse yok. Ama talep de kanıtlanmamış: mavi okyanus bulunmaz, yaratılır |

### 6.2 ERRC ızgarası: The Great Project'in mavi okyanusu nasıl yaratacağı

Mavi Okyanus Stratejisi'nin dört eylemi (Kim & Mauborgne):

| Eylem | The Great Project ne yapar | Kimden ayrışır |
| :--- | :--- | :--- |
| **Kaldır (Eliminate)** | İçeriğin buluta gitmesi; koltuk başına kurumsal fiyat; SOC/CISO'ya yönelik olay yönetimi, ajan/MCP güvenliği | Harmonic, Cyberhaven, Guardian Edge (sunucuda tarama) |
| **Azalt (Reduce)** | Politika karmaşıklığı (3 mod: maskele, uyar, engelle); başlangıçta adaptör sayısı (3 site); kurulum süresi (30 dakika) | Purview, Chrome Enterprise Premium |
| **Yükselt (Raise)** | Doğrulanabilirlik (giden metin görünümü, kanarya testi, açık kod); Türkçe ve TR veri tipi tespiti; çalışan kabulü (maskele, engelleme) | PiiBlocker, ChatShield, Edge DLP |
| **Yarat (Create)** | KVKK kanıt raporu; ERP cari listesinden otomatik sözlük; departman bazlı AI fırsat haritası; tek tuşla ekip şablonu; KVKK danışmanı kanalı | Hiçbiri yapmıyor |

### 6.3 Strateji tuvali

Puan 0–5, yüksek = o faktörde güçlü.

| Faktör | Kurumsal DLP (Harmonic, Cyberhaven) | Platform (Chrome Premium, Edge+Purview) | Ucuz eklenti (PiiBlocker) | TR geçit (kolay.ai, Guardian) | **The Great Project hedefi** |
| :--- | :-: | :-: | :-: | :-: | :-: |
| Fiyat düşüklüğü | 1 | 3 | 5 | 2 | 4 |
| Kurulum hızı | 2 | 3 | 5 | 2 | 5 |
| Tüm AI araçlarını görme | 5 | 2 | 3 | 1 | 4 |
| Maskele + geri doldur | 3 | 0 | 5 | 4 | 5 |
| İçerik bize gelmez | 2 | 2 | 5 | 2 | 5 |
| TR veri tipi ve Türkçe | 1 | 1 | 0 | 5 | 5 |
| KVKK kanıt raporu | 0 | 0 | 0 | 1 | 5 |
| ERP sözlüğü | 0 | 0 | 0 | 0 | 5 |
| Verim / fırsat haritası | 3 (Harmonic) | 0 | 0 | 0 | 4 |
| Ajan / MCP / uygulama güvenliği | 5 | 2 | 0 | 3 | 0 (bilerek) |

The Great Project'in eğrisi hiçbir sütunla çakışmıyor. Son satırı bilerek sıfır bırakmak, kurumsal rafla savaşmamak demek.

### 6.4 Sonuç

Fikir **Türkiye KOBİ'de mavi okyanus adayı, ama okyanus henüz su almamış.** Kanıt yok: ne rakiplerin ne bizim ücretli KOBİ müşterimiz var. Puls pilotu bu yüzden "ürün testi" değil, "pazar var mı" testi. Global KOBİ rafı The Great Project'in modelini (kanıt + verim + kanal) doğruluyor, çünkü orada sadece kalkan satmaya çalışanlar yüzlerce kullanıcıda kaldı.

---

## 7. Geliştirme sürecinde kimden ne alınır

| Referans | Ne alınır | Ne alınmaz |
| :--- | :--- | :--- |
| **Harmonic** | "Engelleme, etkinleştir" konumu; 90 günde ölçülen sonuç iddiası (AI kullanımı arttı, hassas veri maruziyeti düştü) → Faz 0 raporunun şablonu; Usage Intelligence → verim katmanının kurumsal ispatı; uç noktada küçük dil modeli → Faz 1.1 Türkçe NER | Kurumsal fiyat ve SOC entegrasyonu |
| **LayerX / Akamai** | G2 4,9 ve Gartner 4,6: eklenti tabanlı ürünün yüksek memnuniyetle çalışabildiğinin kanıtı; "yeni tarayıcı gerektirmez, mevcut Chrome/Edge'e kurulur" satış dili; çok tarayıcı desteği | Prompt injection, kurumsal tarayıcı alternatifi iddiası |
| **Nightfall** | Yanlış alarm yönetimi G2'de öne çıkan özellik → Faz 1.1 çıkış ölçütü; veri tipi taksonomisi (PII, PHI, finans, kod, sır); şeffaf fiyat sayfası | 300+ çalışan hedefi |
| **Nudge Security** | 750 USD/ay sabit KOBİ fiyatı; "dürtme" (çalışana bağlam içinde kısa uyarı) → "uyar" modunun tasarımı; 200 müşteriyle 3x ARR = küçük biletle büyüme mümkün | E-posta metadata keşfi (TR KOBİ'de M365/Workspace yaygın değil) |
| **Strac** | 10 dakikada ajansız kurulum çıtası; "redaksiyon, kasaya yaz" akışı → eşleme tablosunun bellekte tutulması; G2 4,9 | DSPM ve veritabanı tarama |
| **PiiBlocker** | Geri doldurma UX'i (AES ile şifreli eşleme, 4 saat sonra silme); kategori bazlı "otomatik / sor" politikası; GPO kurulum dokümanı | 521 kullanıcı: kanalsız ücretsiz eklenti dağıtılmıyor. **Uyarı örneği.** |
| **ActivTrak** | Patrona "AI benimseme ve etki" raporu sunumu; "tekrarlayan iş → otomasyon fırsatı" çerçevesi | Kişi bazlı izleme, ekran kaydı (KVKK 2026/2035) |
| **Insightful** | Metadata-only ilkesi; "zaman tasarrufu iddiası yapmıyoruz" dürüstlüğü | Masaüstü ajan |
| **DefensX** | MSP kanalı oyun kitabı: 500 MSP → 7.000 KOBİ; Türk kurucu → olası danışman veya ortak | ABD odaklı fiyatlama |
| **Guardian Edge** | 18 TR veri tipi checksum'lu tespit seti (eşleşmesi gereken çıta); shadow mode; fail-closed seçeneği; HMAC ile paket kilitleme | Sunucuda içerik tarama |
| **Presidio** | Tanıyıcı + doğrulayıcı + anonimleştirici mimarisi; test seti yapısı | Python bağımlılığı (bizde TypeScript) |
| **Perplexity Hybrid** | Yer tutucunun cevapta geri dolması UX'i; "privacy gate" adlandırması | Sadece Mac |
| **Ollama + Open WebUI** | Faz 2 kutu yığını; "bedava alternatif" fiyat çapası | – |

---

## 8. İzlenecek sinyaller (3 ayda bir kontrol)

1. **SHIM Shield** eklentisi çıktı mı? Çıkarsa TR KOBİ rafı ikiye bölünür.
2. **Guardian Edge** pilot'tan fiyatlı ürüne geçti mi? Fiyatı ne?
3. **PiiBlocker** Türkçe veri tipi ekledi mi? Kullanıcı sayısı 521'den nereye gitti?
4. **ESET** tarayıcı chatbot modülü KOBİ paketine girdi mi?
5. **Chrome Enterprise Premium** maskeleme ekledi mi, Türkçe veri tipi ekledi mi?
6. **Akamai Workforce Protector** KOBİ fiyatı açıkladı mı?
7. **Gartner AIUC** kategorisine KOBİ odaklı satıcı girdi mi?

---

## 9. Kaynaklar

- Gartner AI Usage Control pazarı: [Gartner Peer Insights](https://www.gartner.com/reviews/market/ai-usage-control)
- Harmonic: [Unite.AI](https://unite.ai/harmonic-security-raises-50m-series-b-to-expand-us-and-uk-teams), [G2](https://g2.com/products/harmonic-security/reviews)
- LayerX / Akamai: [haber](https://the-coders-blog.pages.dev/akamai-buys-layerx-a-205m-bet-on-ai-browser-security/), [G2](https://www.g2.com/products/layerx-browser-security-platform/reviews)
- Island: [FF News](https://ffnews.com/news/island-announces-400-million-series-f-bringing-valuation-to-6-4-billion-8ad14d83)
- Cyberhaven: [Techleap](https://finder.techleap.nl/news/feed/cyberhaven-raises-100m-hits-1b-valuation), [G2](https://www.g2.com/products/cyberhaven/reviews)
- Nightfall: [G2](https://www.g2.com/products/nightfall-ai/reviews)
- Nudge Security: [basın bülteni](https://www.nudgesecurity.com/press/nudge-security-raises-22-5m-series-a-to-secure-workforce-ai-and-saas)
- Prompt Security: [SiliconANGLE](https://siliconangle.com/2025/08/05/sentinelone-acquires-ai-security-startup-prompt-security/)
- Strac: [G2](https://www.g2.com/products/strac/reviews)
- WitnessAI: [Pulse2](https://pulse2.com/witnessai-58-million-raised-to-expand-globally-and-roll-out-new-security-controls-for-ai-agents)
- Metomic: [SecurityWeek](https://www.securityweek.com/metomic-lands-20-series-a-for-data-security-platform/)
- Aim / Cato: [SecurityWeek](https://www.securityweek.com/cato-networks-acquires-ai-security-firm-aim-security/)
- Lasso: [AI Weekly](https://aiweekly.co/alerts/lasso-security-raises-30m-ships-leap-cpu-only-guardrail-with-sub-5ms-verdicts)
- Knostic: [Virginia Business](https://virginiabusiness.com/knostic-raises-16m-to-secure-generative-ai-data)
- Lakera / Check Point: [SecurityWeek](https://www.securityweek.com/check-point-to-acquire-ai-security-firm-lakera/)
- KOBİ rehberleri: [Rhindon](https://raic.rhindoncyber.com/resources/shadow-ai/smb-buyerguide-2026), [Nudge](https://www.nudgesecurity.com/post/best-shadow-ai-detection-tools), [ShadowLock](https://shadowlock.io/blog/best-ai-dlp-tools/), [Capterra ShadowLock](https://www.capterra.com/p/10048807/ShadowLock/), [Capterra ChatShield](https://www.capterra.com/p/10044878/ChatShield/)
- PiiBlocker: [site](https://www.piiblock.com/), [Chromeboard](https://chromeboard.com/extension/piiblocker-mask-pii-in-ai-nklghhkmhkmckonncilnaohlihfacoee)
- DefensX: [Channel Insider](https://www.channelinsider.com/security/tools-and-platforms/defensx-ai-browser-security-msps/)
- ActivTrak: [basın bülteni](https://www.activtrak.com/news/press-release-momentum-2026/); Insightful: [AI Adoption](https://www.insightful.io/ai-adoption)
- Netskope genAI verisi: [Sacra](https://sacra.com/chat/h/265c3bc4-bd8f-4830-b92f-91ead5e35a2e/)
- Presidio: [hoop.dev](https://hoop.dev/blog/microsoft-signs-multi-year-deal-to-scale-presidio-data-protection-framework); Private AI: [duyuru](https://private-ai.com/?p=8547)
- Ollama: [Noqta](https://noqta.tn/en/news/ollama-65m-series-b-local-ai-open-source-2026); Open WebUI: [IdeaProof](https://ideaproof.io/open-source/project/open-webui)
- Türkiye: [AltaySec ürünler](https://altaysec.com.tr/en/products), [AltaySec TR AI güvenlik listesi](https://altaysec.com.tr/arastirmalar/turkiye-yapay-zeka-guvenligi-sirketleri-2026), [kolay.ai](https://kolay.ai/), [SHIM Product Hunt](https://www.producthunt.com/products/shim/launches), [SHIM Dev.to](https://dev.to/businnect/how-to-secure-ai-applications-without-slowing-them-down-inside-shims-privacy-first-ai-gateway-4aia), [ALP DLP / İTG](https://istanbulticaretgazetesi.com/fikir-okul-sohbetinde-cikti-simdi-veri-sizintisina-set-cekiyor), [Techcareer 2026 TR AI girişimleri](https://www.techcareer.net/blog/turkiyede-yapay-zeka-girisimleri-2026-da-one-cikan-10-startup)
