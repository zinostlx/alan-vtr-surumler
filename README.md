# Alan VTR · Sürümler

Bu depoda yalnızca Alan VTR'nin kurulum dosyaları ve güncelleme bilgisi (`surum.json`) durur. Dosyalar sağdaki **Releases (Sürümler)** sayfasındadır. Kaynak kod bu depoda yoktur.

- **Windows:** `Alan_VTR_Kurulum_<sürüm>.exe`
- **Mac, Apple çipli (M1, M2, M3, M4 …):** `Alan_VTR_<sürüm>_Mac_Apple_cipli.dmg`
- **Mac, Intel:** `Alan_VTR_<sürüm>_Mac_Intel.dmg`

Mac'inizin hangisi olduğunu öğrenmek için: Elma menüsü → Bu Mac Hakkında → "Yonga" satırında "Apple M…" yazıyorsa Apple çipli, "Intel" yazıyorsa Intel paketini indirin. En düşük sürüm: macOS 14 Sonoma.

Uygulama güncellemeleri buradan kendisi denetler; Ayarlar → Araçlar ve güncellemeler.

## Mac'te ilk açılış

Alan VTR, Apple'ın ücretli onayından geçmediği için macOS ilk açılışta uygulamayı durdurur. Uygulama bozuk değildir; macOS yalnızca "internetten indirildi" etiketine bakar. .dmg'nin içindeki **"İlk açılış (önce bunu okuyun).pdf"** aynı adımları resimli anlatır.

1. .dmg dosyasına çift tıklayın, **Alan VTR**'yi yanındaki **Uygulamalar** kısayoluna sürükleyin.
2. Uygulamalar klasöründe Alan VTR'ye çift tıklayın. Şu iki uyarıdan biri çıkabilir:
   - **"hasar görmüş olduğu için açılamıyor"**: **İptal**'e basın (Çöp Sepeti'ne taşımayın), 3. adıma geçin.
   - **"Apple … doğrulayamadı"**: **Bitti**'ye basın; Elma menüsü → Sistem Ayarları → Gizlilik ve Güvenlik → sayfanın altında **Yine de Aç** → şifre ya da Touch ID → **Aç**. 3. adım gerekmez.
3. (Yalnızca "hasar görmüş" dediyse) ⌘ Komut + Boşluk → **Terminal** yazıp Enter. Şu satırı yapıştırıp Enter'a basın:

   ```
   xattr -dr com.apple.quarantine "/Applications/Alan VTR.app"
   ```

   Komut hiçbir şey yazmaz; bu normaldir. Yalnızca Alan VTR'nin "internetten indirildi" etiketini kaldırır, şifre istemez.
4. Alan VTR'yi yeniden açın. Bundan sonra normal açılır. Yeni bir sürümün .dmg'sini indirince bu adımları bir kez daha yapın.
