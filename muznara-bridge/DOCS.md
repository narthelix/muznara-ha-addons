# Muznara Köprüsü

Home Assistant'ı internete açmadan Muznara'ya bağlar.

1. Eklentiyi kur ve **Başlat**.
2. **Web arayüzünü aç**: bir QR ve 6 haneli kod görürsün.
3. Telefonda Muznara › **Evim › Ev ekle › Muznara Köprüsü** → QR'ı tara ya da kodu yaz → evi seç → **Bağla**.
4. Muznara'da hangi alanların cihazlarının geleceğini seç.

- Köprü yalnız **ışık, priz ve kilit** komutlarını çalıştırır; başka hiçbir Home Assistant ayarına dokunmaz.
- Home Assistant'ın şifresi ve token'ı bu cihazdan çıkmaz.
- Köprü Muznara'ya **dışa doğru** bağlanır (`bridge.muznara.com`); evine bir port açman gerekmez.
- Kilidi açmak her seferinde telefonda senin onayınla ve Face ID ile olur; otomasyonlar kilidi asla açmaz.
