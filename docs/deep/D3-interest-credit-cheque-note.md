# D3. Derin İnceleme: Faiz, Kredi, Çek ve Senet / Deep Dive: Interest, Credit, Cheques and Notes

> Hukuki süre, tutar ve ceza hükümleri değişir. Burada **mantık ve yapı** anlatılır; güncel madde ve rakamlar için Çek Kanunu, TTK, İİK ve ilgili tebliğlere bakın. / Legal deadlines and amounts change; verify against current statutes.

## Bölüm A. Faiz matematiği

### A1. Temel formüller
| Kavram | Formül | Örnek |
|---|---|---|
| Basit faiz | F = A × r × t | 10.000 × %10 × 3 yıl = 3.000 |
| Bileşik faiz | F = A × (1+r)ⁿ | 1.000 × 1,10²⁰ ≈ 6.727 |
| Etkin yıllık oran (EAR) | (1 + r_dönem)^(dönem sayısı) − 1 | Aylık %3 → (1,03)¹² − 1 = **%42,58** |
| Reel faiz (Fisher) | (1+nominal)/(1+enflasyon) − 1 | %40 nominal, %50 enflasyon → **−%6,67** |
| 72 kuralı | Katlanma süresi ≈ 72 / r(%) | %6 → 12 yıl; %24 → 3 yıl |
| Gerçek maliyet (APR/YMO) | Masraf ve sigorta dahil iç verim | Kredi karşılaştırma ölçüsü |

**Önemli:** "Aylık %3" yıllık %36 değil, bileşik **%42,58**'dir. Aylık %4,5 faiz yıllık etkin **%69,59**'dur.

![Bileşik büyüme](../img/compound-growth.svg)

1.000 birim: %5'te 30 yılda ≈ 4.322, %10'da ≈ 17.449, %20'de ≈ 237.376. Küçük oran farkı uzun vadede devasa fark yaratır; aynı mantık borçta da geçerlidir.

### A2. Eşit taksitli kredi (amortisman)
Formül: Taksit = A × r / (1 − (1+r)⁻ⁿ)

**Örnek 1: 100.000 birim, aylık %3, 12 ay**
- Aylık taksit ≈ **10.046,21**
- Toplam geri ödeme ≈ 120.554,50; toplam faiz ≈ 20.554,50
| Ay | Taksit | Faiz payı | Anapara payı | Kalan borç |
|---|---|---|---|---|
| 1 | 10.046,21 | 3.000,00 | 7.046,21 | 92.953,79 |
| 2 | 10.046,21 | 2.788,61 | 7.257,59 | 85.696,20 |
| 3 | 10.046,21 | 2.570,89 | 7.475,32 | 78.220,87 |
| … | | | | |
| 12 | 10.046,21 | 292,61 | 9.753,60 | 0,00 |
İlk taksitlerde ödenen paranın büyük kısmı faizdir; erken kapatma bu yüzden ciddi tasarruf sağlar.

**Örnek 2: Aynı 100.000, aylık %3, 24 ay** → taksit ≈ 5.904,74; toplam faiz ≈ **41.713,80** (vade uzayınca taksit düşer, toplam maliyet artar).

**Örnek 3: Aylık %4,5, 36 ay** → taksit ≈ 5.660,58; toplam geri ödeme ≈ **203.780,81** (kredinin yaklaşık iki katı).

### A3. Faiz neden vardır? Neden değişir?
1. **Zaman tercihi:** Bugünkü para değerlidir.
2. **Risk primi:** Borçlu ödeyemeyebilir.
3. **Enflasyon beklentisi:** Paranın alım gücü kaybı telafi edilir.
4. **Vade primi:** Uzun vade belirsizdir.
5. **Likidite tercihi.**
6. **Politika faizi:** Merkez bankası kısa vadeyi belirler, piyasa uzunu fiyatlar.

**Getiri eğrisi (yield curve):** Vadeye göre faiz grafiği. Normalde yukarı eğimli; **ters eğri** (kısa vade > uzun vade) tarihsel olarak resesyon öncesinde sık görülmüştür ama garanti değildir.

**Tahvil fiyatı–faiz ilişkisi:** Faiz artarsa mevcut sabit kuponlu tahvil fiyatı düşer. Vadesi uzun tahvil (yüksek **duration**) daha duyarlıdır.

### A4. Tüketici kredisi tuzakları (yasal ama pahalı)
- Yalnızca aylık faize bakmak; dosya masrafı, hayat sigortası, komisyon eklenince gerçek maliyet artar.
- Asgari ödeme ve kart faizi: Kart borcunu asgari ile kapatmak uzun süre ve yüksek faiz demektir.
- Değişken faiz: Taksit zamanla artabilir.
- Yenileme döngüsü: Borcu borçla kapatmak.
**Bütçe kuralı:** Aylık borç ödemeleri gelirin makul bir bölümünü (ör. üçte birini) aşmasın.

## Bölüm B. Tefecilik, yasa dışı borç ve korunma

### B1. Neden yaygın?
Banka kanalına erişemeyenler, kara listedekiler, acil nakit ihtiyacı. Tefeci hızlı ve belgesiz kredi sunar ama maliyet çok yüksektir.

### B2. Yapı ve işaretler
| İşaret | Anlamı |
|---|---|
| Boş senet/çek imzalatma | Sonradan tutar yazılması riski |
| Tapu/araç/kimlik rehni | Haksız teminat |
| Önceden kesinti ("masraf" adı altında) | Gizli faiz |
| Tehdit, taciz, aile/işyerine baskı | Ayrıca suç |
| Sürekli yenileme (dönmeyen borç) | Borç tuzağı |

### B3. Hukuki dayanaklar (özet)
- Tefecilik TCK md. 241; tehdit, şantaj, hürriyetten yoksun kılma, konut dokunulmazlığı ihlali ayrı suçlardır.
- Faiz üst sınırları: 3095 sayılı Kanun ve Merkez Bankası'nca belirlenen oranlar (güncel oranlar için TCMB).
- İcra aşamasında borçlu **itiraz, şikâyet, menfi tespit, istirdat** gibi yollara sahiptir.
- Boş imzalı belgeyi doldurma sahtecilik/güveni kötüye kullanma olabilir.

### B4. Mağdur için adımlar
1. Konuşmaları ve ödemeleri kaydedin, dekont saklayın.
2. Tehdit varsa 112/155'e ve savcılığa gidin.
3. Avukattan menfi tespit/istirdat seçeneklerini sorun.
4. Banka kanalında yapılandırma isteyin; kredi birlikleri ve yasal mikro-finans alternatiflerine bakın.

## Bölüm C. Çek (ayrıntılı)

### C1. Çekin yapısı
**Zorunlu unsurlar (genel):** "Çek" ibaresi, kayıtsız şartsız havale, ödenecek tutar, muhatap banka, ödeme yeri, düzenleme yeri ve tarihi, keşidecinin imzası. Eksiklik varsa çek geçersiz sayılabilir.

**Taraflar:** Keşideci (çeki yazan), muhatap banka, lehtar/hamil (tahsil eden), ciranta (devreden).

**Çek türleri:** Nama yazılı, emre yazılı, hamile yazılı (ciro ile devredilir, hamile yazılıda teslimle devir); çizgili çek (yalnızca bankaya/müşteriye ödenir), hesaba geçirilecek çek.

### C2. Ciro türleri
| Ciro | Anlamı |
|---|---|
| Tam ciro | Devralan kişi belirtilir |
| Beyaz ciro | Sadece imza; taşıyana ödenir |
| Tahsil cirosu | Vekil sıfatıyla tahsil için |
| Rehin cirosu | Teminat amaçlı |

### C3. İşleyiş
```mermaid
flowchart TD
    A[Keşideci çek verir] --> B[Lehtar/ciranta devreder]
    B --> C[Hamil süresi içinde bankaya ibraz eder]
    C --> D{Hesapta karşılık?}
    D -- Var --> E[Ödeme]
    D -- Yok --> F[Karşılıksızdır işlemi]
    F --> G[Hamil: icra / dava]
    F --> H[Keşideci: bankalar çek defteri vermez, yaptırımlar]
```
- **İbraz süresi:** Düzenleme–ödeme yeri aynıysa kısa (günler), farklıysa uzun (ay); yurt dışı çeklerde daha uzun. Süre geçince bankanın ödeme yükümlülüğü kalkmasa da hamilin rücu hakları sınırlanır.
- **Banka ödeme sorumluluğu:** Kanunda belirlenen tutara kadar karşılık yoksa bile banka ödeme yapar ve keşideciden tahsil eder (sistem güncel tutarlar belirler).
- **Vadeli çek:** İleri tarihli çek hukuken ibrazda ödenir. Taraflar arasında vade yazılsa da bankaya erken ibraz edilebilir; bu yüzden çek "vade aracı" değildir.
- **Zamanaşımı:** Çek hakları kısa zamanaşımına tabidir (altı ay mertebesinde süreler), mevzuatı kontrol edin.
- **Kaybolma/çalınma:** Bankaya yazılı bildirim, ilgili mahkemeye iptal/ödeme yasağı başvurusu.

### C4. Çek riskleri ve sahtecilik türleri
- **Sahte imza / sahte çek yaprağı:** Resmî belgede sahtecilik.
- **Değiştirilmiş (tahrif) çek:** Tutar/isim değişikliği.
- **Çek kitingi (check kiting):** İki hesap arasında gerçek karşılık olmadan çekle sahte bakiye yaratma (suç).
- **Ciro zincirinde kopukluk veya sahte ciro.**
- **Muvazaalı çek (malı teslim etmeden çek alma):** Çek bir ticari işlem karşılığı değilse; çek tek başına ödeme garantisi vermez.
- **"Çek karşılığı kredi" (çek-senet tefeciliği).**

### C5. Güvenli kullanım rehberi
1. Çekin ön-arka yüzünü, imzayı, tarihi, tutar yazı-rakam uyumunu kontrol edin.
2. Keşidecinin çek karnesi/yasak durumunu bankadan öğrenin.
3. Çizgi çekmek, çeke "hesaba geçirilecek" yazmak çalınma halinde riski azaltır.
4. Karşılıksız çıkarsa süreleri kaçırmadan hukuki yola başvurun.
5. Çeki depozito/güvence olarak vermeyin; teminat için yazılı sözleşme kullanın.

## Bölüm D. Senet / Bono (ayrıntılı)

### D1. Unsurlar (TTK'ya göre özet)
1. Senet metninde "bono" veya "emre yazılı senet" ibaresi (dilde ifade),
2. Belirli bir bedeli ödeme vaadi (kayıtsız şartsız),
3. Vade (belirtilmezse görüldüğünde ödenir sayılır),
4. Ödeme yeri,
5. Kime veya kimin emrine ödeneceği,
6. Düzenleme tarihi ve yeri,
7. Borçlunun imzası.
Eksik unsur varsa senet "kambiyo senedi" niteliğini yitirebilir; adi borç senedi olarak kalabilir.

### D2. Vade çeşitleri
Görüldüğünde ödenir · görüldükten belirli süre sonra · düzenleme tarihinden belirli süre sonra · belirli bir günde.

### D3. Aval ve ciro
- **Aval:** Üçüncü kişinin borçluya kefil gibi imza vermesi; aval veren borcun tamamından sorumlu olabilir.
- **Ciro:** Senedin devri; ciranta da sorumlu olur (ciro silsilesi kesintisiz olmalı).

### D4. Takip yolları (özet)
- **Kambiyo senetlerine özgü haciz yolu:** Senedin kambiyo vasfı varsa hızlı takip. Borçlu ödeme emrine karşı kısa sürede şikâyet ve borca itiraz yollarını kullanır (genelde 5 gün; kontrol edin).
- **Genel haciz yolu veya dava:** Kambiyo vasfı yoksa.
- **Protesto:** Ödeme reddi resmen tespiti; bazı rücu hakları için gerekli olabilir.
- **Zamanaşımı:** Bonoda vadeden itibaren belirli yıllar (TTK'da; güncel süre için mevzuat).

### D5. Riskler ve tuzaklar
- **Boş senet imzalatma:** Sonradan doldurma tutar ve vade ihtilafı; ispat yükü tartışması.
- **Teminat senedi:** Asıl borç sözleşmesine bağlı; sebepsiz ödeme talebi menfi tespit konusu olabilir.
- **Senedin zayi olması:** İptal davası.
- **Faiz gizleme:** Senet bedeline faiz eklemek, "masraf" yazmak.
- **Sahte senet:** Sahtecilik suçu; imza incelemesi (grafoloji/uzman raporu).

### D6. Çek ve senet karşılaştırma
| Özellik | Çek | Senet (Bono) |
|---|---|---|
| Düzenleyen | Keşideci (hesap sahibi) | Borçlu |
| Üçüncü taraf | Muhatap banka şart | Banka yok |
| Vade | Görüldüğünde ödenir | Vadeli olabilir |
| Karşılık | Hesapta olmalı | Borçlunun malvarlığı |
| Yaptırım | Çek Kanunu, banka kayıtları | Takip, icra, hukuki yollar |
| Kullanım | Hızlı ödeme aracı | Kredi/borç senedi |

## Bölüm E. Kısa pratik senaryolar
1. **Çekle mal sattınız, çek karşılıksız çıktı:** Ibraz tarihi, karşılıksızdır şerhi, keşideciye/ciro edenlere rücu; icra takibi.
2. **Kardeşinize senet verdiniz, "güvence" denildi:** Yazılı sözleşme ve senet ilişkisi; ödenince senedi geri alın ve ödeme belgesi isteyin.
3. **Tefeci boş çek istiyor:** Vermeyin; yasal kredi arayın; baskı varsa savcılık.

## English summary
Interest: simple, compound, EAR, real (Fisher) and the rule of 72; 3%/month equals 42.58% a year compounded. Amortization worked examples show most early installments are interest. Usury and illegal lending rely on blank cheques/notes, hidden fees and threats; victims should keep records, report threats and seek legal remedies. Cheques: unconditional order to pay on presentation; presentation periods, endorsement types, bank liability, kiting and forgery. Promissory notes: seven essential elements, aval (guarantee), summary enforcement procedures, protest and limitation periods. Always verify current statutory numbers.
