# Устанавливаем 3x-ui панель для VLESS и сертификаты на 10 лет

## 📚 Описание

Этот скрипт автоматически устанавливает:
1. Панель **3X-UI**.
2. Самоподписной **SSL-сертификат** для доступа к панели по **https** сроком на **10 лет**.

## 🛠️ Что будет установлено?
- **OpenSSL**
- **QRencode**
- **3X-UI**

## 🚀 Как использовать?

### 1. Установка 3X-UI + сертификаты панели на 10 лет
```bash
sudo apt update && sudo apt install -y git curl openssl qrencode systemd && rm -rf ~/self-signed-cert-3x-ui && git clone https://github.com/swr8bit/self-signed-cert-3x-ui.git && cd self-signed-cert-3x-ui && chmod +x self_signed_cert.sh && sudo ./self_signed_cert.sh
```

### =======================================================
### 2 Установка - только сертификаты панели
```bash
sudo apt update && sudo apt install -y git curl openssl systemd && rm -rf ~/self-signed-cert-3x-ui && git clone https://github.com/swr8bit/self-signed-cert-3x-ui.git && cd self-signed-cert-3x-ui && chmod +x self_signed_cert_only.sh && sudo ./self_signed_cert_only.sh
```
