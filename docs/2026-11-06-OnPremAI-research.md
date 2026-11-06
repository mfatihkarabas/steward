# On-Prem Gizlilik Odaklı AI (KOBİ Ofis Asistanı): Araştırma ve Karar

**Tarih:** 2026-11-06
**Durum:** Ham fikir, ilk araştırma turu. Birincil sinyal (müşteri görüşmesi) henüz sıfır.
**Fikir sahibinin çerçevesi:** Pazar önce Türkiye, sonra İngiltere (GB). Ürün yazılım + donanım ya da sadece yazılım. Hedef KOBİ, kullanım ağırlıklı olarak genel ofis çalışanı.

---

## 1. Tek cümlede fikir

Verisini dışarı çıkaramayan veya çıkarmak istemeyen şirketlerde, ofis çalışanının ChatGPT'ye yapıştırdığı her şeyi (müşteri listesi, sözleşme, bordro, hasta notu) şirketin kendi kutusunda veya sunucusunda çalışan bir AI asistanına taşımak.

---

## 2. Neden şimdi: Türkiye'ye özgü üç gerçek koz

| Koz | Kanıt | Okuma |
| :--- | :--- | :--- |
| **KVKK yurt dışı aktarım kuralı (m.9, 2024)** | 1 Haziran 2024'ten beri yurt dışına aktarım için yeterlilik kararı, standart sözleşme (imzadan sonra 5 iş günü içinde Kurum'a bildirim) veya diğer güvenceler gerekiyor. Bildirim yapmayana idari para cezası var. ([Erdem & Erdem](https://www.erdem-erdem.av.tr/bilgi-bankasi/kisisel-verilerin-korunmasi-kanununda-neler-degisti)) | Bir çalışanın ChatGPT'ye müşteri verisi yapıştırması teknik olarak yurt dışına aktarım. KOBİ'nin OpenAI ile Türk standart sözleşmesi imzalayıp bildirmesi pratikte olmuyor. Yani çoğu ofis bugün sessizce kural dışında. |
| **KVKK "İş Yerlerinde Üretken Yapay Zekâ" duyurusu (5 Mart 2026)** | Kurum "Gölge Yapay Zekâ (Shadow AI)" riskini adıyla andı. Kurumsal politika, erişim kuralları ve anonimleştirme öneriyor. ([Erdem & Erdem](https://www.erdem-erdem.av.tr/bilgi-bankasi/is-yerlerinde-uretken-yapay-zeka-araclarinin-kullanimi-baslikli-kisisel-verileri-koruma-kurumu-duyurusu-yayimlandi)). Ayrıca Kasım 2025'te Üretken YZ rehberi yayımlandı. ([KVKK](https://www.kvkk.gov.tr/Icerik/8547/uretken-yapay-zeka-ve-kisisel-verilerin-korunmasi-rehberi-15-soruda)) | Satış konuşmasının ilk cümlesi hazır: "Kurum bu riski adıyla söyledi, sizin politikanız ne?" |
| **Microsoft Copilot'un ülke içi işleme listesinde Türkiye yok** | Microsoft 15 ülkeye ülke içi Copilot veri işleme sözü verdi. UK var, Türkiye yok. ([Microsoft](https://www.microsoft.com/en-us/microsoft-365/blog/2025/11/04/microsoft-offers-in-country-data-processing-to-15-countries-to-strengthen-sovereign-controls-for-microsoft-365-copilot/)) | Türkiye'de en büyük rakibin "veri ülkede kalır" diyememesi gerçek bir açık. UK'de bu koz 2026 sonunda büyük ölçüde kapanıyor. |

**Talep tarafı (TÜİK 2026):** Bireylerde üretken AI kullanımı bir yılda %19.2'den %37.6'ya çıktı. Şirketlerde herhangi bir AI kullanımı ise sadece %14. ([CHIP / TÜİK](https://www.chip.com.tr/guncel/turkiye-yapay-zekaya-alisti-kullanim-bir-yilda-neredeyse-ikiye-katlandi_184345.html))
→ Çalışanlar kullanıyor, şirketler resmi olarak kullanmıyor. Aradaki fark tam olarak gölge AI ve bu fikrin pazarı.

---

## 3. Tezin zayıf noktaları (şeytanın avukatı)

1. **KOBİ gizlilik için para ödemez, cezadan korkarsa öder.** KVKK denetimi KOBİ'de seyrek. "Mahremiyet" tek başına satmaz. "Denetimde/şikâyette elinde politika ve kayıt olsun" satar. *(Bu benim yargım, saha ile doğrulanmalı.)*
2. **Genel ofis kullanımı = ChatGPT ve Copilot ile kafa kafaya.** Kullanıcı kaliteyi kıyaslar. Lokal 7–30B modeller frontier modellerin gerisinde, Türkçede fark daha da açık. Türkçe kurumsal dokümanlarda RAG ile yapılan bir çalışmada en iyi açık model (Trendyol-LLM-8B) %75–82 doğruluk aldı ama Qwen2.5-7B'den 14 kat yavaştı. Getirme (retrieval) tavanı %57'de kaldı. ([arXiv 2609.28007](https://arxiv.org/pdf/2609.28007))
3. **Fiyat çapası düşük.** Copilot Business kullanıcı başı aylık $21 (2026 sonuna kadar $18 promosyon), ChatGPT Business $25. ([aipricing.guru](https://www.aipricing.guru/compare/copilot-m365-business-vs-chatgpt-team/)) 10 kişilik bir ofis buluta ayda yaklaşık $210–250 ödüyor. Lokal çözüm bunun üstüne çıkamaz.
4. **Donanım ekonomisi kötüleşiyor.** DRAM fiyatları 2026'da katlandı. DGX Spark $3,999'dan $4,699'a çıktı (Şubat 2026), 64 GB sürümü $4,999'dan başlıyor. AMD'nin 128 GB'lık Halo kutusu $3,999. ([Tom's Hardware](https://www.tomshardware.com/desktops/mini-pcs/nvidia-dgx-spark-gets-18-percent-price-increase-as-memory-shortages-bite-founders-edition-now-usd4-699-up-from-usd3-999), [Hypebeast](https://hypebeast.com/2026/5/amd-ryzen-ai-halo-workstation-priced-from-3999), [TweakTown](https://www.tweaktown.com/news/113885/nvidias-new-dgx-spark-has-half-the-ram-and-costs-more-than-the-original-128gb-model-did-at-launch/index.html)) Türkiye'de ithalat maliyeti ve kur riski eklenince donanım satmak stok, garanti ve servis yükü demek.
5. **İşletim sistemi tehdidi.** Windows ve macOS cihaz üstü modelleri bedava getiriyor. 2–3 yıl içinde "lokal sohbet" bir özellik olur, ürün olmaz. *(Tahmin.)*
6. **KOBİ'de IT yok.** Kutuyu kim kuracak, güncelleyecek, yedekleyecek? Bu, ürünün yarısı.

---

## 4. Rakip haritası

### Türkiye
| Oyuncu | Ne yapıyor | Segment | Not |
| :--- | :--- | :--- | :--- |
| [kolay.ai](https://kolay.ai/) | Kurumsal AI geçidi: OpenAI/Claude/Gemini/açık modelleri tek katmandan yönetim, politika, TL fatura; on-prem/VPC opsiyonu | Kurumsal | Fiyat ve müşteri açıklanmamış |
| [KobiGPT](https://komunite.com.tr/fabrika/urunler/kobigpt) (X Mind Solutions) | Şirket içi veriyle soru-cevap, departman asistanları; KVKK için on-prem opsiyonu | KOBİ + kurumsal | En doğrudan rakip; fiyat yok, ölçeği belirsiz |
| Mio Bilişim, Nexsol, Yazılım Koçu, Sora Yazılım, Anıt Medya vb. | Proje bazlı "şirkete özel LLM" kurulumu | Karışık | Ajans/entegratör modeli, ürünleşmemiş |
| Trendyol LLM, Turkish-Gemma vb. | Açık Türkçe modeller ([Webrazzi](https://webrazzi.com/2026/02/18/turkce-icin-one-cikan-acik-kaynak-modeller/)) | Altyapı | Rakip değil, bizim hammaddemiz |

**Okuma:** Türkiye'de "KVKK uyumlu şirket içi AI" diyen çok kişi var ama hepsi ya kurumsal ya da proje/danışmanlık. KOBİ'ye kutudan çıkıp çalışan, fiyatı belli bir ürün görmedim.

### İngiltere ve global
| Oyuncu | Ne yapıyor | Para / fiyat |
| :--- | :--- | :--- |
| [Lemony](https://techcrunch.com/2025/06/11/uptime-industries-wants-to-boost-localized-ai-usage-with-an-ai-in-a-box-called-lemony-ai/) (Uptime Industries, ABD) | Sandviç boyutunda AI kutusu, 5 kullanıcı, 75B'ye kadar model, ekip bazlı benimseme | $2M seed (True Ventures), **$499/ay** |
| [Locai Labs](https://datacentrenews.uk/story/locai-labs-launches-on-premises-ai-appliance-for-uk) (UK) | Locai One cihazı (RTX PRO 6000), kendi modelleri; UK hükümeti deniyor | £1m pre-seed ([Pulse](https://www.pulse.bot/ai/news/locai-raises-1m-to-develop-its-off-cloud-ai-infrastructure-7a42dc63-ac00-4979-bd58-8fbc69fe5426/)), Ağustos 2026 lansman |
| [Deliverance AI](https://thenextweb.com/news/deliverance-ai-stealth-sovereign-enterprise-ai) (UK) | On-prem/air-gapped ajan işletim sistemi, HPE ve DGX ile | £6M ARR (şirket beyanı), kurumsal |
| [Prem AI](https://www.runtimewire.com/article/swiss-ai-startup-prem-ai-100m-series-a), [Cohere North](https://ai2.work/blog/cohere-raises-500m-for-behind-the-firewall-enterprise-ai) | Kurumsal özel AI platformu | $100M / $500M |
| QNAP, yerel MSP'ler | AI sunucusu veya "biz kurarız" hizmeti | Donanım marjı |
| **Perplexity Hybrid Compute** (1 Eyl 2026) | Görev bulut ile Mac'teki lokal model arasında bölünüyor. Cihaz üstü "privacy gate" isim, adres, hesap no, kimlik gibi verileri buluta gitmeden maskeliyor, cevapta geri dolduruyor; admin kuralları ve denetim kaydı var. ([Unite.AI](https://www.unite.ai/perplexity-launches-hybrid-compute-on-mac-with-local-privacy-gate/)) Ayrıca DGX Spark üstünde tamamen lokal "Portable Computer" (26 Ağu 2026). ([Techzine](https://www.techzine.eu/news/infrastructure/143850/perplexity-opts-for-local-ai-with-nvidia/)) | Pro/Max/Enterprise aboneliği; sadece Apple silicon Mac (24 GB+) |

### Okyanus rengi
- **Büyük şirket:** 🔴 Kırmızı. Cohere, Microsoft, HPE+Nvidia ve Deliverance burada.
- **KOBİ, global:** 🟣 Erken ve kalabalıklaşıyor. Lemony ve Locai fonlandı ama küçükler, kazanan yok.
- **KOBİ, Türkiye:** 🟢 Ürün olarak boş, hizmet olarak kalabalık. Yerel avantaj (KVKK, Türkçe, TL fatura, saha kurulum) gerçek.

---

## 5. Segment analizi

| | Küçük (1–20 kişi) | Orta (20–250) | Büyük (250+) |
| :--- | :--- | :--- | :--- |
| Acı | Var ama farkında değil | Var, KVKK danışmanı soruyor | Çok var |
| Bütçe | Çok düşük | Orta | Yüksek |
| IT kapasitesi | Yok | 1–2 kişi veya dış MSP | Ekip var, kendileri kurar |
| Satış döngüsü | Kısa ama churn yüksek | 1–3 ay | 6–18 ay, ihale |
| Rakip baskısı | ChatGPT bedava sürümü | Az | Çok |
| **Uygunluk** | Zayıf (tek başına) | **En iyi** | Kurucu profiline uymuyor |

**Öneri:** "Genel ofis çalışanı" ürünün kullanıcısı olabilir ama satış kapısı çok geniş. İlk 20 müşteri için tek bir **regüle meslek** seç:
- **Hukuk büroları:** Sözleşme ve dilekçe, avukat-müvekkil gizliliği. Ödeme gücü iyi.
- **Mali müşavir (SMMM) ofisleri:** Yüzlerce müşterinin bordro ve vergi verisi; ofisler birbirini tanıyor, ağ etkisi güçlü.
- **Özel klinik ve poliklinikler:** Sağlık verisi özel nitelikli kişisel veri, ceza riski en yüksek.
- **Sigorta acenteleri ve İK/bordro firmaları:** Yoğun kişisel veri, tekrarlı ofis işi.

Ürün aynı genel ofis asistanı kalır. Değişen sadece ilk 5 hazır şablon ve satış dili.

---

## 6. Ürün şekli önerisi

**Saf on-prem yerine "KVKK geçidi + lokal model" hibriti:**

1. Kutuda (veya müşterinin sunucusunda) küçük bir lokal model çalışır.
2. Çalışan bir şey sorduğunda kişisel veri (TC kimlik, isim, IBAN, sağlık bilgisi) **lokalde maskelenir**.
3. Gerekirse maskelenmiş istek frontier modele (Claude, GPT, Gemini) gider, cevap geri gelince maskeler lokalde geri doldurulur.
4. Tamamen hassas işler (bordro, hasta dosyası) hiç dışarı çıkmadan lokal modelde çözülür.
5. Her istek loglanır → KVKK denetiminde "politika + kayıt" hazırdır.

**Neden:** Kalite problemini (madde 3.2) çözer, donanım ihtiyacını küçültür (dev model değil, maskeleme ve hafif işler için model yeter) ve "gölge AI'ı yasakla" yerine "gölge AI'ı güvenli hale getir" der. Çalışan ChatGPT kalitesinden vazgeçmek zorunda kalmaz.

**Uyarı: Bu mimari tek başına moat değil.** Perplexity Eylül 2026'da tam olarak bu yöntemi (lokal maskeleme + bulut akıl yürütme + geri doldurma) Mac'te shipledi. Mimari doğrulandı ama kopyalanabilir. Ayrışma şunlarda olmalı:
- **Ofis geneli, cihaz başı değil:** Perplexity kişi ve Mac başına çalışıyor. Türk ofisleri ağırlıkla Windows; tek bir ofis kutusu herkese hizmet eder.
- **Türkçe ve Türkiye'ye özgü veri:** TC kimlik no, VKN, IBAN, SGK sicil, e-fatura alanları için yerel tanıma.
- **KVKK çıktısı:** Kurum'un istediği politika, erişim kuralları ve kayıtları hazır rapor olarak vermek.
- **Mesleğe özel akışlar:** SMMM, hukuk veya klinik şablonları; genel asistan değil iş bitiren akış.
- **TL fatura ve yerel kurulum ortağı.**

**Donanım kararı:** Stok tutma. Sadece yazılım sat, 2–3 sertifikalı donanım referansı ver (DGX Spark, Ryzen AI Max mini PC, mevcut bir sunucu). Kurulumu yerel bilgisayarcı/MSP ortakları yapsın, onlara gelir payı ver. "Kutu" istendiğinde ortak satar.

**Fiyat hipotezi:** Kullanıcı başı aylık Copilot'un altında veya eşit (örnek: $15–20), artı tek seferlik kurulum ücreti (ortak kazanır). Lemony'nin $499/ay/5 kullanıcı fiyatı üst sınır referansı.

---

## 7. İngiltere (GB) notu

- UK GDPR var ama Microsoft Copilot 2026 sonunda UK içinde işleme yapacak. Gizlilik argümanı UK'de Türkiye'deki kadar keskin değil.
- UK'de ayrışma "veri ülkede kalır" değil, **"token başı ücret yok, sabit maliyet"** ve **regüle meslekler** (solicitor, muhasebeci, GP klinikleri) olur.
- FSB: Küçük firmaların %55'i AI kullanıyor (2023'te %20), %92'si risklerden endişeli. ([Resultsense / FSB](https://www.resultsense.com/news/2026-06-23-fsb-ai-trust-gap-42bn/))
- Rakip olarak Locai Labs ve Lemony zaten orada. GB'yi ikinci pazar tutmak doğru, ama oraya Türkiye'deki ürünle değil, UK'deki regüle bir meslek için yerelleştirilmiş şablonla gidilmeli.

---

## 8. Skor kartı (1–5)

| Faktör | Puan | Gerekçe |
| :--- | :---: | :--- |
| Acının gerçekliği | 4 | KVKK m.9 + Kurum'un gölge AI duyurusu |
| Ödeme isteği (KOBİ) | 2 | Gizlilik tek başına satmıyor, korku ve kayıt satıyor |
| Türkiye'de rekabet boşluğu | 4 | Ürünleşmiş KOBİ çözümü yok |
| Global rekabet boşluğu | 2 | Lemony, Locai fonlu |
| Teknik risk | 3 | Türkçe lokal model kalitesi; hibrit yaklaşım riski düşürür |
| Donanım/operasyon riski | 2 | DRAM krizi, kur, servis; yazılım-öncelikli ile 3'e çıkar |
| Moat | 2 | Yerel kanal ağı + mesleğe özel şablonlar dışında zayıf |
| Kurucu uyumu | 3 | Yazılım tarafı güçlü; saha/kanal satışı yeni bir kas |
| **Toplam** | **22/40** | |

---

## 9. Karar (YC gözüyle)

**PIVOT / DARALT.** "KOBİ'ler için on-prem genel AI" olarak bu bir donanım-artı-hizmet işi ve YC'nin para koyacağı bir şey değil: yatay, sermaye yoğun, moat'sız, ve OS satıcıları bedavaya getirecek.

Ama **"Türk KOBİ'leri için KVKK uyumlu AI çalışma alanı: gölge AI'ı yasaklama, güvenli hale getir"** yatırım konuşulabilir bir wedge:
- Türkiye'ye özgü düzenleyici bir neden var (m.9 + Mart 2026 duyurusu) ve en büyük rakip (Copilot) Türkiye'de ülke içi işleme sunmuyor.
- Hibrit maskeleme mimarisi kalite problemini çözüyor.
- Tek bir regüle meslekle başlarsan (öneri: mali müşavirler veya hukuk büroları) dağıtım ağızdan ağıza yürüyebilir.

**Okyanus:** Türkiye KOBİ'de mavi ama sığ. Global'de mor.

---

## 10. Koddan önceki 2 haftalık test

1. **15 görüşme:** 5 hukuk bürosu, 5 SMMM ofisi, 5 klinik. Tek soru seti:
   - Çalışanlarınız ChatGPT'ye müşteri verisi yapıştırıyor mu? Bunu nereden biliyorsunuz?
   - KVKK danışmanınız veya denetçiniz bunu hiç sordu mu?
   - Copilot/ChatGPT Business'a para veriyor musunuz? Vermiyorsanız neden?
   - "Veri dışarı çıkmaz, kalite ChatGPT gibi, kayıt tutulur" ürünü için kullanıcı başı aylık ne öderdiniz?
2. **Lead magnet:** Ücretsiz "Gölge AI KVKK risk testi" (10 soruluk form + PDF rapor). Ölçüm: 2 haftada form dolduran ofis sayısı.
3. **Eşik:** 15 görüşmeden en az 5'i "pilot yaparız" derse ve en az bir meslek grubu öne çıkarsa build. Yoksa fikri UK regüle meslekler açısından yeniden değerlendir.

---

## 11. Açık sorular

- İlk meslek hangisi: mali müşavir mi, hukuk bürosu mu, klinik mi?
- Hibrit (maskeleyip buluta gönderen) model kabul edilebilir mi, yoksa "hiçbir şey dışarı çıkmaz" mı vaat edilecek? İkincisi kaliteyi ve donanım maliyetini zorlar.
- Kanal ortağı modeli (yerel bilgisayarcı/MSP) mi, doğrudan satış mı?
- KVKK yeterlilik kararı ve standart sözleşme pratiği bir KVKK avukatıyla doğrulanmalı (bu rapor hukuki görüş değildir).
