# 🚀 VPS Reinstaller

Reinstalador automático de VPS com interface interativa.
Suporta múltiplos sistemas Linux e Windows.

## ⚡ Instalação Rápida

**Comando único - detecta automaticamente sua arquitetura:**

bash <(wget -qO- https://raw.githubusercontent.com/nandoslayer/vps-reinstaller/main/install.sh)

Ou com curl:

bash <(curl -fsSL https://raw.githubusercontent.com/nandoslayer/vps-reinstaller/main/install.sh)

---

## 📥 Download Manual

Se preferir baixar manualmente:

### Para Intel/AMD (x86_64) - Maioria das VPS

wget https://github.com/nandoslayer/vps-reinstaller/releases/latest/download/vps-reinstaller-x86_64
chmod +x vps-reinstaller-x86_64
./vps-reinstaller-x86_64

### Para ARM64 (Oracle Cloud, AWS Graviton)

wget https://github.com/nandoslayer/vps-reinstaller/releases/latest/download/vps-reinstaller-aarch64
chmod +x vps-reinstaller-aarch64
./vps-reinstaller-aarch64

---

## 📦 Sistemas Disponíveis

### 🐧 Ubuntu LTS
- 24.04 LTS (Noble Numbat)
- 22.04 LTS (Jammy Jellyfish)
- 20.04 LTS (Focal Fossa)
- 18.04 LTS (Bionic Beaver)

### 🐧 Debian
- Debian 13 (Trixie)
- Debian 12 (Bookworm)
- Debian 11 (Bullseye)
- Debian 10 (Buster)
- Debian 9 (Stretch)
- Debian 8 (Jessie)
- Debian 7 (Wheezy)

### 🐧 Kali Linux
- rolling
- dev
- experimental

### 🐧 Alpine Linux
- 3.16
- 3.17
- 3.18
- edge

### 🐧 CentOS
- 7
- 8
- 9-stream

### 🐧 AlmaLinux
- 8
- 9

### 🐧 Rocky Linux
- 8
- 9

### 🐧 Fedora
- 42
- 43

---

### 🪟 Windows
- Windows 10
- Windows 11
- Windows Server 2012 R2
- Windows Server 2016
- Windows Server 2019
- Windows Server 2022

---

## 🎯 Como funciona

1. Execute o comando de instalação
2. Escolha o sistema operacional
3. Escolha a versão desejada
4. Configure a senha root (ou gere automaticamente)
5. Confirme a reinstalação
6. Aguarde e reconecte via SSH ou RDP

---

## ⚠️ AVISOS IMPORTANTES

- ESTE PROCESSO APAGA TODOS OS DADOS DA VPS
- Faça BACKUP antes de executar
- O acesso SSH será interrompido temporariamente
- O processo pode levar de 5 a 40 minutos
- Guarde a senha gerada

---

## 🏗️ Arquiteturas Suportadas

| Arquitetura | Binário |
|------------|--------|
| x86_64 (Intel/AMD) | vps-reinstaller-x86_64 |
| aarch64 (ARM 64-bit) | vps-reinstaller-aarch64 |

---

## ❓ Problemas Comuns

Permission denied:
chmod +x vps-reinstaller-*

Cannot execute binary file:
uname -m

x86_64 → use vps-reinstaller-x86_64  
aarch64 → use vps-reinstaller-aarch64  

---

## 🆘 Suporte

- 🐙 [GitHub Issues](https://github.com/nandoslayer/vps-reinstaller/issues)
- 📢 [Canal no Telegram](https://t.me/paineis)

---

## 📄 Licença

Uso livre. Use por sua conta e risco.
