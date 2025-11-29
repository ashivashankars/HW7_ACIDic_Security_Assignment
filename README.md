# 📘 PKI Infrastructure + Tomcat HTTPS — CMPE 272

Team ACIDic:
- Archana Shivashankar
- Pratham Rajesh
- Venkata Rama Gowri Preetam Gunisetty
- Zach Xie

This project demonstrates how to build a complete Public Key Infrastructure (PKI) using OpenSSL and configure Tomcat 9 to serve HTTPS using certificates created by this PKI.

The setup includes:

- **Root Certificate Authority (Root CA)**
- **Intermediate Certificate Authority (Signing CA)**
- **Server TLS Certificate (for Tomcat HTTPS)**
- **Tomcat HTTPS deployment on macOS**

---

## 📁 Directory Structure

```markdown
pki/
├── root/
│ ├── certs/
│ │ └── root.crt.pem
│ ├── crl/
│ ├── csr/
│ ├── index.txt
│ ├── index.txt.attr
│ ├── index.txt.attr.old
│ ├── index.txt.old
│ ├── newcerts/
│ │ ├── 1000.pem
│ │ └── 1001.pem
│ ├── openssl.cnf
│ ├── private/
│ │ └── root.key.pem
│ ├── serial
│ └── serial.old
└── int/
├── certs/
│ ├── app.local.crt.pem
│ ├── app.local.fullchain.crt.pem
│ ├── int-chain.crt.pem
│ └── int.crt.pem
├── crl/
├── csr/
│ ├── app.local.csr.pem
│ └── int.csr.pem
├── index.txt
├── index.txt.attr
├── index.txt.attr.old
├── index.txt.old
├── newcerts/
├── openssl.cnf
├── private/
│ ├── app.local.key.pem
│ └── int.key.pem
├── serial
├── serial.old
└── server-san.ext
```
