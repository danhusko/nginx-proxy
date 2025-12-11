---
marp: true
theme: neobeam-ecobeam
paginate: true
footer: "**Prostředí Webu**
  **NGINX**"
---

<!-- _class: title -->

# Prostředí Webu <br> Ukázka aplikace proxy serveru pomoci Nginx

## Jaroslav Štěpán, Ondřej Kačírek, Daniala Hušková

### 18.12.2025

---

<!-- header: 'Úvod do NGINX' -->

- Vysoce výkonný bezplatný webový server, reverzní proxy a load balancer.
- Navržený pro vysokou propustnost, nízkou paměťovou náročnost a práci s velkým počtem souběžných spojení (ruský programátor Igor Sysoev, rok 2004)
- Použití: webhosting, API brány, CDN, microservices, reverse proxy vrstva.
- Napsán s cílem překonat webový server Apache

---

<!-- header: 'Proxy Server' -->
### Forward proxy
- umístěna mezi klientem a internetem  
- klient → Proxy → Internet  
- použití:
  - filtrování  
  - anonymizace  
  - bezpečnost  

### Reverse proxy
- stojí mezi klientem a backend serverem  
- klient → Reverse Proxy (NGINX) → Aplikační / backend server  
- použití:
  - load balancing  
  - cache  
  - TLS terminace  
  - ochrana backendu

---

<!-- header: 'NGINX Reverse Proxy vs Forward Proxy' -->
