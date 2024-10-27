# Ubuntu Kurulum Rehberi - Ahmed SULTAN

Ubuntu 24.04'ün kurulumuna yönelik kapsamlı bir rehberi burada bulabilirsiniz.

1. [**Ubuntu Sistem Gereksinimleri**](#ubuntu-sistem-gereksinimleri)
2. [**Ubuntu Kuruluma Hazırlık**](#ubuntu-kuruluma-hazırlık)
   - [2.1 Görüntünün İndirilmesi](#21-görüntünün-indirilmesi)
   - [2.2 Görüntüyü USB'ye Yazdırma](#22-görüntüyü-usbye-yazdırma)
   - [2.3 BIOS Ayarları](#23-bios-ayarları)
3. [**Ubuntu 24.04 Kurulumu**](#ubuntu-2404-kurulumu)
   - [3.1 Dil Seçimi](#31-dil-seçimi)
   - [3.2 Sistem Yükleyiciyi Başlatma](#32-sistem-yükleyiciyi-başlatma)
   - [3.3 Klavye Düzeni](#33-klavye-düzeni)
   - [3.4 Yazılım Seçimi](#34-yazılım-seçimi)
   - [3.5 Disk Bölümlendirme Nasıl Yapılır](#35-disk-bölümlendirme-nasıl-yapılır)
   - [3.6 Bootloader Bölümü Oluşturma](#36-bootloader-bölümü-oluşturma)
   - [3.7 Root Bölümü Oluşturma](#37-root-bölümü-oluşturma)
   - [3.8 Home Bölümü Oluşturma](#38-home-bölümü-oluşturma)
   - [3.9 Zaman Dilimi Seçimi](#39-zaman-dilimi-seçimi)
   - [3.10 Kullanıcı Oluşturma](#310-kullanıcı-oluşturma)
   - [3.11 Sistemin Yüklenmesi](#311-sistemin-yüklenmesi)
   - [3.12 Yeniden Başlatma](#312-yeniden-başlatma)
4. [**Sonuçlar**](#sonuçlar)

---

### 1. Ubuntu Sistem Gereksinimleri

Kuruluma başlamadan önce dikkate almanız gerekenler:

- Bilgisayarınızı güç kaynağına bağlayın.
- En az 20 GB boş depolama alanına sahip olduğunuzdan emin olun.
- Kurulum ortamı olarak bir DVD veya USB sürücüsüne sahip olun.
- Önemli verilerinizin güncel bir yedeğini aldığınızdan emin olun.

#### Minimal Sistem Gereksinimleri:
- 2 GHz çift çekirdekli işlemci
- 4 GB RAM
- 50 GB disk alanı
- 1024x768 çözünürlüğe sahip VGA ekran
- Kurulum medyası için bir CD/DVD sürücüsü veya USB bağlantı noktası
- İnternet bağlantısı önerilir.

---

### 2. Ubuntu Kuruluma Hazırlık

Kuruluma geçmeden önce her şeyi hazırlamalıyız.

#### 2.1 Görüntünün İndirilmesi
- Ubuntu web sitesine giderek Masaüstü sürümünü indirin.
  
   > **![Görüntü 1](https://github.com/user-attachments/assets/14a57c47-76d0-4faa-bbab-b74875501157)** (Ubuntu web sitesinden indirirken)

#### 2.2 Görüntüyü USB'ye Yazdırma
- İndirilen ISO dosyasını **Rufus** gibi bir araç ile USB belleğe yazdırın.
  
   > **![Görüntü 2](https://github.com/user-attachments/assets/459dc9f7-7a0a-4707-94f4-acc3d2caae2a)** (Rufus ayarları yapılırken)

#### 2.3 BIOS Ayarları
- Bilgisayarınızı USB'den başlatın. Başlangıçta **F12** veya **ESC** gibi tuşlara basarak başlatma menüsünden USB'yi seçin.

   > **![Görüntü 3](https://github.com/user-attachments/assets/65cdddd7-d396-45e0-a006-88076d3a302b)** (BIOS ayar ekranı görünümü)

---

### 3. Ubuntu 24.04 Kurulumu

Bilgisayarınızı yeniden başlattıktan sonra kuruluma başlayacağız.

#### 3.1 Dil Seçimi
- Karşınıza çıkan ilk pencerede dili seçin.
  
   > **![Görüntü 4](https://github.com/user-attachments/assets/02486d94-e0de-4bdd-bd22-195d02cb9d50)** (Dil seçimi ekranı)

#### 3.2 Sistem Yükleyiciyi Başlatma
- **Install Ubuntu** seçeneğini seçerek yükleyiciyi başlatın.
  
   > **![Görüntü 5](https://github.com/user-attachments/assets/53abf43c-8ea0-41ef-b67c-422123fc7f65)** (Install Ubuntu ekranı)

#### 3.3 Klavye Düzeni
- Klavye düzeninizi seçin ve **Devam** butonuna tıklayın.
  
   > **![Görüntü 6](https://github.com/user-attachments/assets/e5742653-b912-4c6d-9b9d-9569b0699a04)** (Klavye düzeni seçimi ekranı)

#### 3.4 Yazılım Seçimi
- Normal veya Minimal kurulum seçeneklerinden birini seçin. Ayrıca, güncellemeleri indir ve üçüncü parti yazılımları yükle seçeneklerini etkinleştirin.

   > **![Görüntü 7](https://github.com/user-attachments/assets/95f87462-75f0-48b2-aa9e-69fe52dd1051)** (Yazılım seçimi ekranı)

#### 3.5 Disk Bölümlendirme Nasıl Yapılır
- **Diğer Seçenekler** seçeneğini seçin ve disk bölümlerinizi ayarlayın.

   > **![Görüntü 8](https://github.com/user-attachments/assets/3b6e7e62-1663-41ef-b76a-7dbe7cb3b7e6)** (Disk bölümlendirme ekranı)

#### 3.6 Bootloader Bölümü Oluşturma
- **/boot** bölümü oluşturmak için, tür olarak **ext4** ve bağlama noktası olarak **/boot** seçin.

   > **![Görüntü 9](https://github.com/user-attachments/assets/13189d8e-70e9-4523-a1bf-49826d058eee)** (Boot bölümü oluşturma)

#### 3.7 Root Bölümü Oluşturma
- **/ (kök)** bölümü için yeterli alan ayırın ve tür olarak **ext4** seçin.

   > **![Görüntü 10](https://github.com/user-attachments/assets/66e9c73a-05a7-4de8-b14f-b1540f0de60b)** (Root bölümü oluşturma)

#### 3.8 Home Bölümü Oluşturma
- Kullanıcı dosyalarınız için **/home** bölümünü oluşturun.

#### 3.9 Zaman Dilimi Seçimi
- Zaman diliminizi seçin ve **Devam** butonuna tıklayın.

#### 3.10 Kullanıcı Oluşturma
- Adınızı ve parolanızı girerek kullanıcı hesabınızı oluşturun.

#### 3.11 Sistemin Yüklenmesi
- Yükleyici tamamlanana kadar bekleyin. Bu işlem birkaç dakika sürebilir.

#### 3.12 Yeniden Başlatma
- Her şey tamamlandığında, bilgisayarınızı yeniden başlatın.

---

### Sonuçlar
Ubuntu'yu başarıyla kurdunuz! Artık Ubuntu'nun sunduğu olanaklardan faydalanmaya hazırsınız.

---

**Teşekkürler**: Bu çalışmada bize ilham veren **BULANIK MANTIK LAB. Dr. Öğr. Üyesi FEVZİ DAŞ** hocamıza teşekkür ederim.

---

Bu rehberde Ubuntu 24.04 kurulum adımlarını bulacaksınız.

[![Kurulum Videosunu İzle](https://github.com/user-attachments/assets/f9b6a8b4-2466-47e2-abdd-78df16444156)](https://youtu.be/fSY4e3YqIiQ")

### Açıklama
Bu video, Ahmed SULTAN tarafından Ubuntu 24.04 kurulum sürecini adım adım açıklamaktadır.







