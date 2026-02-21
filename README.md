cat > README.md << 'EOF'
# Aegis Tunnel

> Zero-Trust Secure Tunnel Service built with Java, Spring Boot & WireGuard.

---

## 🚀 Vision

Aegis Tunnel is a Zero-Trust secure tunneling service designed to protect internal services from public internet exposure while allowing authorized remote access.

It separates:

- **Data Plane** → Encrypted traffic (WireGuard)
- **Control Plane** → Identity, device management, policies (Spring Boot)

This project is built for learning, architecture demonstration, and security-focused backend engineering.

---

## 🎯 Problem It Solves

Modern teams work remotely and host services in the cloud.

Common problems:
- Internal APIs exposed publicly
- Over-permissive VPNs
- Lack of device-level control
- No proper access revocation

Aegis Tunnel provides:
- Encrypted tunnels
- Device-based access control
- Zero-Trust policy enforcement
- Instant revocation capability

---

## 🏗️ High-Level Architecture

Client Device  
   ↓ (Encrypted Tunnel)  
WireGuard Gateway  
   ↓  
Internal Services (Private Network)

Control Plane:
Spring Boot API manages users, devices, and policies.

---

## 🛡️ Security Principles

- Zero-Trust by default
- Least privilege access
- Device binding
- Key rotation capability
- No direct public exposure of internal services

---

## 📌 Scope (MVP)

- User authentication (JWT)
- Device registration (peers)
- WireGuard config generation
- Access policy enforcement
- Device revocation
- Audit logging

---

## 🚫 Out of Scope (Initial Version)

- Consumer VPN for general browsing
- Anonymous internet routing (Tor-style)
- Multi-region HA setup
- Mobile native app

---

## 🧠 Learning Goals

- Networking fundamentals
- WireGuard integration
- Secure system design
- Threat modeling
- Enterprise-grade backend architecture

---

## 🛠️ Tech Stack (Planned)

- Java 21
- Spring Boot 3
- Spring Security
- PostgreSQL
- Docker
- WireGuard

---

## 📅 Status

Phase 0 – Foundations

---

## ⚠️ Disclaimer

This project is for educational and architectural demonstration purposes.
Not intended for production use without further hardening.

---

Author: Johnny Telles
EOF