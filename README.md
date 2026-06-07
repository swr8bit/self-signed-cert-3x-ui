# Установка 3x-ui панели с ssl сертификатами на 10 лет

## 📚 Описание

Этот скрипт автоматически устанавливает:
1. Панель **3X-UI**.
2. Самоподписной **SSL-сертификат** для доступа к панели по **https** сроком на **10 лет**.

## 🛠️ Что будет установлено?
- **OpenSSL**
- **QRencode**
- **3X-UI 2.9.4**

---

## 🚀 Как использовать?

### 1. Установка 3X-UI + сертификаты панели на 10 лет
```bash
sudo apt update && sudo apt install -y git curl openssl qrencode systemd && rm -rf ~/self-signed-cert-3x-ui && git clone https://github.com/swr8bit/self-signed-cert-3x-ui.git && cd self-signed-cert-3x-ui && chmod +x self_signed_cert.sh && sudo ./self_signed_cert.sh
```
#### Если вы не root
```bash
sudo -i bash -c "apt update && apt install -y git curl openssl qrencode systemd && rm -rf ~/self-signed-cert-3x-ui && git clone https://github.com/swr8bit/self-signed-cert-3x-ui.git && cd self-signed-cert-3x-ui && chmod +x self_signed_cert.sh && ./self_signed_cert.sh"
```

### 2 Установка - только сертификаты панели
```bash
sudo apt update && sudo apt install -y git curl openssl systemd && rm -rf ~/self-signed-cert-3x-ui && git clone https://github.com/swr8bit/self-signed-cert-3x-ui.git && cd self-signed-cert-3x-ui && chmod +x self_signed_cert_only.sh && sudo ./self_signed_cert_only.sh
```
#### Если вы не root
```bash
sudo -i  bash -c "apt update && apt install -y git curl openssl systemd && rm -rf ~/self-signed-cert-3x-ui && git clone https://github.com/swr8bit/self-signed-cert-3x-ui.git && cd self-signed-cert-3x-ui && chmod +x self_signed_cert_only.sh && ./self_signed_cert_only.sh"
```

---

### Важное уведомление об авторских правах
Данный проект включает в себя исходный код, созданный пользователем anten-ka (https://github.com/anten-ka). Этот код не содержит явной лицензии на использование. В соответствии с действующим законодательством об авторском праве, все права на оригинальный код принадлежат его создателю.

Мои собственные изменения и дополнения к этому коду распространяются под лицензией GNU General Public License v3.0 or later. Полный текст лицензии доступен в файле LICENSE

### Зависимости и лицензии

Данный скрипт устанавливает и настраивает следующие сторонние компоненты:

- **[3X-UI](https://github.com/MHSanaei/3x-ui)** — панель управления Xray. Распространяется под лицензией **GPL-3.0**.
- **[Xray-core](https://github.com/XTLS/Xray-core)** — прокси-платформа. Распространяется под лицензией **MPL-2.0** (Mozilla Public License 2.0).

Оригинальные лицензии этих проектов применяются к их коду и сохраняют силу. Данный скрипт является лишь установщиком и не изменяет условия лицензирования указанных проектов.
