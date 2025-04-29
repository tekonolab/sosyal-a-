# Kullanıcı Sosyal Ağ Sistemi (Red-Black Tree & Graph Tabanlı)

Bu proje, bir sosyal ağ simülasyonu olarak tasarlanmıştır. Her kullanıcı benzersiz bir kimliğe sahiptir ve kullanıcılar arasında arkadaşlık ilişkileri kurulabilir. Sistem, kullanıcıları **Red-Black Tree (Kırmızı-Siyah Ağaç)** içinde sıralı ve dengeli bir şekilde saklar. Ayrıca kullanıcılar arasında arkadaşlıklar bir **graf** yapısıyla temsil edilir.

## 🚀 Özellikler

- ✅ Yeni kullanıcı ekleme (Red-Black Tree ile)
- ✅ Kullanıcılar arası arkadaşlık kurma (Graf bağlantısı)
- ✅ Derinlik-sınırlı DFS (Depth-First Search) ile arkadaş listesi
- ✅ İki kullanıcı arasında ortak arkadaş analizi
- ✅ Bir kullanıcının etki alanını hesaplama (kaç kullanıcıya ulaşabildiğini bulur)
- ✅ Topluluk tespiti (bağlı bileşenleri bulur)
- ✅ Veriyi dosyaya yazma (`veriseti.txt`)
- ✅ Dosya içeriğini ekrana yazdırma

---

## 🛠 Derleme ve Çalıştırma

```bash
gcc sosyal_ag.c -o sosyal_ag
./sosyal_ag
Program Akışı
Kullanıcı sayısı girilir.

Her kullanıcı için ID girilir ve ağaç yapısına eklenir.

Arkadaşlık ilişkileri girilir ve grafik yapısı oluşturulur.

DFS ile belirli derinliğe kadar arkadaşlar listelenir.

Ortak arkadaşlar bulunur.

Etki alanı hesaplanır.

Topluluk (bağlantılı bileşen) analizi yapılır.

Tüm kullanıcı ve arkadaşlık verileri veriseti.txt dosyasına yazılır ve ekrana bastırılır.# Kullanicilar
KULLANICI 1
KULLANICI 2
KULLANICI 3

# Arkadaslik Iliskileri
ARKADAS 1 2
ARKADAS 2 3
Kullanılan Veri Yapıları
Red-Black Tree (Kırmızı-Siyah Ağaç):

Kullanıcılar ID'ye göre sıralanır.

Dengeli ağaç yapısı sayesinde arama ve ekleme işlemleri O(log n) sürede gerçekleşir.

Graf (Adjacency List Yaklaşımı):

Arkadaşlıklar çift yönlüdür.

Her kullanıcının arkadaslar[] dizisinde bağlantıları tutulur.Bilinen Eksiklikler
Kullanıcı silme işlemi bulunmamaktadır.

arkadaslar[] dizisi sabit boyutludur (MAX_KULLANICI), taşma kontrolü yapılmaz.

Ortak arkadaş analizi O(n²) karmaşıklıktadır (küçük ağlar için yeterli).Kac kullanici eklemek istersiniz? 3
Kullanici ID girin: 1
Kullanici ID girin: 2
Kullanici ID girin: 3

Kac arkadaslik iliskisi tanimlanacak? 2
Arkadaslik (id1 id2): 1 2
Arkadaslik (id1 id2): 2 3

DFS ile 2 derinliğe kadar arkadaşları listele:
Baslangic kullanici ID: 1
Kullanici 1 derinlik 0
Kullanici 2 derinlik 1
Kullanici 3 derinlik 2

---

İstersen bu README dosyasını `.md` formatında çıktı olarak da sağlayabilirim. README’yi proje klasörüne kaydetmek ister misin?
