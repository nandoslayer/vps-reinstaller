# 🚀 VPS Reinstaller

Reinstalador automático de VPS com interface interativa. Suporta Ubuntu e Debian.

## ⚡ Instalação Rápida

**Comando único - detecta automaticamente sua arquitetura:**

```bash
bash <(wget -qO- https://raw.githubusercontent.com/nandoslayer/vps-reinstaller/main/install.sh)
```

Ou com curl:
```bash
curl -sSL https://raw.githubusercontent.com/nandoslayer/vps-reinstaller/main/install.sh | bash
```

---

## 📥 Download Manual

Se preferir baixar manualmente:

### Para Intel/AMD (x86_64) - Maioria das VPS
```bash
wget https://github.com/nandoslayer/vps-reinstaller/releases/latest/download/vps-reinstaller-x86_64
chmod +x vps-reinstaller-x86_64
./vps-reinstaller-x86_64
```

### Para ARM64 (Oracle Cloud, AWS Graviton)
```bash
wget https://github.com/nandoslayer/vps-reinstaller/releases/latest/download/vps-reinstaller-aarch64
chmod +x vps-reinstaller-aarch64
./vps-reinstaller-aarch64
```

---

## 📦 Sistemas Disponíveis

### Ubuntu LTS:
- ✅ 24.04 LTS (Noble Numbat) - Suporte até 2029
- ✅ 22.04 LTS (Jammy Jellyfish) - Suporte até 2027
- ✅ 20.04 LTS (Focal Fossa) - Suporte até 2025
- ✅ 18.04 LTS (Bionic Beaver) - EOL 2023

### Debian:
- ✅ Debian 12 (Bookworm) - Stable
- ✅ Debian 11 (Bullseye) - Oldstable
- ✅ Debian 10 (Buster) - Oldoldstable

---

## 🎯 Como funciona

1. **Execute o comando de instalação** (detecta sua arquitetura automaticamente)
2. **Escolha o sistema operacional** (Ubuntu ou Debian)
3. **Escolha a versão** que deseja instalar
4. **Configure a senha root** (ou gere uma automaticamente)
5. **Confirme** e aguarde 5-10 minutos
6. **Reconecte via SSH** com a nova senha

---

## ⚠️ AVISOS IMPORTANTES

- 🔥 Este programa **APAGA TODOS OS DADOS** da VPS
- 💾 **Faça BACKUP** antes de executar
- 🔌 Você vai **perder acesso SSH** durante a reinstalação
- ⏰ Aguarde **5-10 minutos** após executar
- 🔑 **Anote a senha** gerada (se não criar uma personalizada)

---

## 🏗️ Arquiteturas Suportadas

| Arquitetura | Binário | Provedores |
|-------------|---------|------------|
| Intel/AMD 64-bit | `vps-reinstaller-x86_64` | DigitalOcean, Vultr, Linode, Hetzner, AWS |
| ARM 64-bit | `vps-reinstaller-aarch64` | Oracle Cloud, AWS Graviton, Azure ARM |

---

## 🔐 Verificação de Integridade (Opcional)

Para verificar se o binário não foi adulterado:

```bash
# Baixe o binário e o checksum
wget https://github.com/nandoslayer/vps-reinstaller/releases/latest/download/vps-reinstaller-x86_64
wget https://github.com/nandoslayer/vps-reinstaller/releases/latest/download/vps-reinstaller-x86_64.sha256

# Verifique
sha256sum -c vps-reinstaller-x86_64.sha256
```

Se aparecer "OK", está tudo certo! ✅

---

## ❓ Problemas Comuns

### "Permission denied"
```bash
chmod +x vps-reinstaller-*
```

### "cannot execute binary file"
Você baixou o binário errado! Verifique sua arquitetura:
```bash
uname -m
# x86_64 = use vps-reinstaller-x86_64
# aarch64 = use vps-reinstaller-aarch64
```

### Não consigo baixar do GitHub
Verifique se você tem `wget` ou `curl` instalado:
```bash
# Instalar wget (Debian/Ubuntu)
apt install wget
```

---

## 🆘 Suporte

Abra uma issue: https://github.com/nandoslayer/vps-reinstaller/issues

---

## 📄 Licença

Uso livre. Use por sua conta e risco.
