# Görüşme Rehberi: Puls Elektronik (İlk Müşteri Görüşmesi)

**Tarih:** 2026-11-06
**Fikir:** Gölge AI kalkanı / KVKK ve gizlilik uyumlu AI çalışma alanı (bkz. `2026-11-06-OnPremAI-research.md`)
**Görüşmeci:** Fatih (şirkette daha önce mühendis olarak çalıştı)

---

## 1. Şirket hakkında bildiklerimiz

- **Puls Elektronik Sistemleri Makina San. A.Ş.**, Hadımköy / Arnavutköy, İstanbul. Kuruluş 2008, listelerde 10+ çalışan görünüyor. ([pulselectronic.com](https://pulselectronic.com), [Manuzone](https://manuzone.com/companies/show/puls-elektronik-sistemleri-makina-sanayi-ic-ve-dis-ticaret-anonim-sirketi_vX4xVlyGnz))
- **Ürünler:** Checkweigher ve metal dedektör kombinasyonu, gravimetrik/volumetrik dozajlama, yük hücreleri, transmitter ve indikatörler, silo tartım, statik elektrik gidericiler, web temizleyiciler, vinç/asansör aşırı yük sınırlayıcıları.
- **Müşteri sektörleri:** Gıda, kozmetik, ilaç, kâğıt ve plastik baskı, vinç/asansör. İhracat yapıyor.

**Fatih'in içeriden bildikleri (2026-11-06):**
- **Çalışan:** 30–50 kişi. (Listelerdeki "10+" eski veya eksik.)
- **Karar vericiler:** Patron ve bir genel müdür. İkisiyle de konuşmak gerekiyor.
- **IT:** İçeriden biri yapıyor. → Pilotun teknik muhatabı o; görüşmede mutlaka tanış.
- **Bilgisayarlar:** Windows. Tarayıcı ağırlıkla Chrome, Edge kullanan da olabilir. → Eklenti ikisini de desteklemeli.
- **Microsoft 365 / Google Workspace / merkezi yönetim:** Bilinmiyor. → Görüşmede IT sorumlusuna sor.
- **Kod, PCB tasarımı, şartnameler:** Şirket sunucusunda.
- **Müşteri NDA'ları:** Bilinmiyor. → Görüşmede sor.
- **AI kullanımı:** Fatih'in zamanında yoktu. Şu an kullanıldığını biliyor ve **patronun mahremiyet yüzünden bundan memnun olmadığını düşünüyor.** Bu güçlü bir sinyal ama ikinci elden; görüşmede patronun kendi ağzından, somut bir olayla doğrulanmalı (bkz. soru 8).
- **Yazılı AI kuralı:** Yok.
- **Pilot:** 3–5 bilgisayar uygun.

**Görüşmede ek sorular (IT sorumlusuna):**
- Microsoft 365 mi, Google Workspace mi kullanılıyor? Bilgisayarlar domain'e bağlı mı, Chrome/Edge merkezden yönetilebiliyor mu?
- Hangi ERP / muhasebe programı var (Logo, Mikro, Netsis, Nebim...)? Cari hesap listesini (müşteri ve tedarikçi adları) CSV olarak alabilir miyiz? → Maskeleme sözlüğünün ana kaynağı bu.
- Sunucudaki müşteri/proje klasörleri nasıl adlandırılmış? (Sadece klasör adları, içerik değil.)

---

## 2. Bu görüşme neyi test eder, neyi test etmez

Puls bir **regüle meslek değil, endüstriyel üretici.** Bu yüzden:

- **Muhtemel acı KVKK değil, ticari sır ve müşteri gizliliği.** Mühendisin firmware kodunu, devre şemasını veya bir ilaç müşterisinin teknik şartnamesini ChatGPT'ye yapıştırması. İlaç ve gıda müşterileri genelde gizlilik sözleşmesi (NDA) imzalatır.
- KVKK tarafı ikincil: personel bordrosu, müşteri iletişim bilgileri, ihracat yazışmaları.
- Yani bu görüşme raporun ana hipotezini (hukuk/SMMM/klinik) değil, **yeni bir hipotezi** test ediyor: *"İhracatçı endüstriyel KOBİ'ler ticari sır yüzünden AI kullanımını kontrol etmek ister mi?"* Bu iyi bir şey. Raporda olmayan bir segmenti açabilir.

---

## 3. Tanıdık riski (en önemli kural)

Seni tanıyorlar ve kırmak istemezler. "Harika fikir, alırız" cevabı **sıfır bilgi** taşır. Bunu aşmak için:

1. **Fikrini anlatma, önce onların hayatını sor.** Ürün sadece son 5 dakikada.
2. **Gelecek değil geçmiş sor.** "Kullanır mısınız?" yerine "En son ne zaman ...?"
3. **İltifatı not alma, olayı not al.** "Çok mantıklı" değil, "geçen ay şu oldu" değerli.
4. **Sonunda somut bir taahhüt iste** (zaman, erişim veya para). Taahhüt yoksa cevap "hayır"dır.

---

## 4. Kiminle konuşmalı

İdeal olarak 30–45 dakika, mümkünse ayrı ayrı:
- **Patron / genel müdür:** Karar ve bütçe sahibi. Ticari sır kaygısı burada.
- **1–2 mühendis (Ar-Ge, yazılım/firmware):** AI'ı en çok kullanan ve en riskli veriyi tutan grup.
- **Satış / ihracat:** Teklif, müşteri yazışması ve çeviri için AI kullanıyor olabilir.
- **Muhasebe / İK (varsa):** KVKK tarafı.

Tek kişiyle görüşebiliyorsan patronla başla, sonra "mühendislerle 15 dakika konuşabilir miyim?" diye iste. Bu da bir taahhüt sinyali.

---

## 5. Soru seti

### A. Bugünkü AI kullanımı (geçmiş davranış)
1. Şirkette şu an kim, hangi AI araçlarını kullanıyor? (ChatGPT, Gemini, Copilot, DeepL...)
2. Son kullandığınız zamanı anlatır mısınız? Ne için kullandınız?
3. Bu araçlar için şirket para ödüyor mu, yoksa herkes kendi hesabıyla mı kullanıyor?
4. Bir şirket kuralı ya da yazılı politika var mı? Kim koydu, ne zaman?

### B. Hassas veri
5. AI'a hiç yapıştırılmaması gereken bilgiler sizin için neler? (kod, şema, teklif fiyatları, müşteri şartnamesi...)
6. Birinin bunları yapıştırıp yapıştırmadığını bugün nereden bilirsiniz?
7. Müşterilerinizle (özellikle ilaç ve gıda) gizlilik sözleşmeniz var mı? İçinde üçüncü taraf yazılım veya bulut ile ilgili bir madde var mı?

### C. Olaylar ve kaygılar
8. Bu konuda hiç bir şey yaşandı mı? Bir müşteri sordu mu, bir denetimde gündeme geldi mi?
9. Rakiplerinizin ya da sektörden birinin başına gelen bir şey duydunuz mu?
10. KVKK danışmanınız veya mali müşaviriniz AI kullanımı hakkında hiç bir şey söyledi mi?

### D. Para ve karar
11. Son 1 yılda güvenlik veya IT için yeni bir şeye para verdiniz mi? Ne kadar, karar nasıl verildi?
12. Bu tür bir harcamaya kim karar verir, kimin onayı gerekir?
13. Bugün bu problemi çözmek için bir şey denediniz mi (yasaklamak, bir araç, eğitim)?

### E. Kapanış: ürünü şimdi anlat (2–3 cümle)
> "Çalışanlar ChatGPT'yi aynen kullanmaya devam ediyor. Ama tarayıcıdaki bir eklenti, gizli bilgiyi buluta gitmeden maskeliyor, cevap gelince geri dolduruyor ve kimin neyi gönderdiğinin kaydını tutuyor. İsterseniz çok gizli işler için ofiste lokal çalışan bir kutu da var."

14. Bu sizin için hangi durumda işe yarardı, hangi durumda yaramazdı?
15. En büyük çekinceniz ne olurdu? (Tarayıcı eklentisine güven, maliyet, kurulum...)

### F. Somut sonraki adım (birini mutlaka iste)
- "Ücretsiz bir gölge AI kontrolü yapalım mı? 2 hafta boyunca 3 bilgisayarda sadece *neyin* gönderildiğini sayan (içeriği kaydetmeyen) bir araç çalıştıralım, sonunda size rapor vereyim."
- Ya da: "Bir mühendisinizle 15 dakika konuşabilir miyim?"
- Ya da: "Sektörden bu konuyu dert edebilecek 2 firma tanıtabilir misiniz?"

---

## 6. Sinyaller

| Güçlü sinyal | Zayıf sinyal |
| :--- | :--- |
| Somut bir olay anlatıyorlar (müşteri sordu, kod yapıştırıldı) | "Mantıklı, olabilir" |
| Zaten bir şey denemişler (yasak, politika, araç) | "Bizde öyle bir şey olmaz" |
| Müşteri NDA'sında yazılım/bulut maddesi var | Kimse AI kullanmıyor |
| Pilot veya mühendis görüşmesine hemen evet diyorlar | "Sonra konuşalım", tarih yok |
| Fiyat soruyorlar | Sadece teknik merak |

---

## 7. Görüşme notu şablonu

- **Kiminle, rolü:**
- **AI kullanımı (kim, ne için, ücretli mi):**
- **Hassas veri türleri:**
- **Anlatılan somut olaylar (alıntı):**
- **Mevcut çözüm / politika:**
- **Bütçe ve karar verici:**
- **Ürüne tepki ve çekinceler:**
- **Alınan taahhüt:**
- **Benim yorumum (görüşmeden sonra, ayrı yaz):**
