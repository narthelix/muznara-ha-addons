# Muznara Home Assistant eklentileri

Home Assistant'ta: **Ayarlar › Eklentiler › Eklenti Mağazası › ⋮ › Depolar** →
`https://github.com/narthelix/muznara-ha-addons`

| Eklenti | Ne yapar |
|---|---|
| [Muznara Köprüsü](muznara-bridge/DOCS.md) | Home Assistant'ı internete açmadan Muznara'ya bağlar |

Bu depo yalnız eklenti tanımlarını tutar; imaj `ghcr.io/narthelix/muznara-bridge`
(çok mimarili, cosign imzalı). Doğrulamak için:

```sh
cosign verify ghcr.io/narthelix/muznara-bridge:1.0.0 \
  --certificate-identity-regexp 'https://github.com/narthelix/muznara-bridge/' \
  --certificate-oidc-issuer https://token.actions.githubusercontent.com
```
