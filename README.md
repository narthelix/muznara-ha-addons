# Muznara Home Assistant eklentileri

Home Assistant'ta: **Ayarlar › Eklentiler › Eklenti Mağazası › ⋮ › Depolar** →
`https://github.com/narthelix/muznara-ha-addons`

| Eklenti | Ne yapar |
|---|---|
| [Muznara Köprüsü](muznara-bridge/DOCS.md) | Home Assistant'ı internete açmadan Muznara'ya bağlar |

Bu depo yalnız eklenti tanımlarını tutar; imaj `ghcr.io/narthelix/muznara-bridge`
(çok mimarili, cosign imzalı).

**1.4.0 ve sonrası** bu depodaki `cosign.pub` anahtarıyla imzalıdır:

```sh
cosign verify --key https://raw.githubusercontent.com/narthelix/muznara-ha-addons/main/cosign.pub   ghcr.io/narthelix/muznara-bridge:1.4.0
```

**1.3.1 ve öncesi** GitHub Actions kimliğiyle anahtarsız imzalıdır:

```sh
cosign verify ghcr.io/narthelix/muznara-bridge:1.3.1   --certificate-identity-regexp 'https://github.com/narthelix/muznara-bridge/'   --certificate-oidc-issuer https://token.actions.githubusercontent.com
```
