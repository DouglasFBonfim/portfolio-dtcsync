# Portfolio — DTCSync — agente Windows com autoatualização

> Public case study only. **No source code** is published here (client/production systems remain private).  
> Estudo de caso público. **Sem código-fonte** (sistemas de cliente/produção permanecem privados).  
> Caso de estudio público. **Sin código fuente** (sistemas de cliente/producción permanecen privados).

---

## 🇧🇷 Português

### DTCSync — agente Windows no posto

**Role / Papel / Rol:** Desenvolvimento completo (desktop + web local + empacotamento)  
**Stack:** `Python, HTML/CSS, PyInstaller, GitHub Releases, Windows services, PostgreSQL`

#### Problem / Problema
Cada posto tem PostgreSQL próprio e módulos contratados diferentes. Sem um agente local, a matriz não monitora o posto, não cria roles com segurança e não aplica só o que foi liberado.

#### Solution / Solução / Solución
Agente Windows (`ConfigServer.ini` + painel `localhost:9010`) com heartbeat/watchdog como serviço, autoatualização via GitHub, sync de módulos (Dashboard, PontoBR, Rodoil, relatórios etc.), grants no Postgres do cliente e envio de ocorrências para a API central.

#### Highlights
- Configuração local (INI + web) — banco nunca vem da API
- Watchdog / serviço Windows e multi-instância por porta
- Sync condicionado aos módulos contratados
- Autoatualização a partir de releases


---

## 🇬🇧 English

### DTCSync — on-site Windows agent

**Role / Papel / Rol:** Full development (desktop + local web + packaging)  
**Stack:** `Python, HTML/CSS, PyInstaller, GitHub Releases, Windows services, PostgreSQL`

#### Problem / Problema
Each site has its own PostgreSQL and licensed modules. Without a local agent, HQ cannot monitor the site, create DB roles safely, or apply only what was contracted.

#### Solution / Solução / Solución
A Windows agent (`ConfigServer.ini` + `localhost:9010` panel) with heartbeat/watchdog as a service, GitHub auto-update, module sync (Dashboard, PontoBR, Rodoil, reports, etc.), Postgres grants on the customer DB and occurrence push to the central API.

#### Highlights
- Local config (INI + web) — DB never comes from the API
- Watchdog / Windows service and multi-instance by port
- Sync gated by contracted modules
- Auto-update from releases


---

## 🇪🇸 Español

### DTCSync — agente Windows en el puesto

**Role / Papel / Rol:** Desarrollo completo (desktop + web local + empaquetado)  
**Stack:** `Python, HTML/CSS, PyInstaller, GitHub Releases, Windows services, PostgreSQL`

#### Problem / Problema
Cada cliente tiene su PostgreSQL y módulos contratados. Sin agente local, la matriz no monitorea, no crea roles con seguridad ni aplica solo lo liberado.

#### Solution / Solução / Solución
Agente Windows (`ConfigServer.ini` + panel `localhost:9010`) con heartbeat/watchdog como servicio, autoactualización vía GitHub, sync de módulos, grants en Postgres del cliente y envío de ocurrencias a la API central.

#### Highlights
- Configuración local (INI + web)
- Watchdog / servicio Windows y multi-instancia
- Sync según módulos contratados
- Autoactualización desde releases


---

## Notes / Observações / Notas

- Author: **Douglas Francisco Bonfim**
- Related private implementation (not public): `dtcsync` / `DTCSync`
- Companion cases: `dtcsync-server`, `dtcsyncclient`, `dtcsyncandroid`
- No credentials, customer data, hostnames, or proprietary payloads are included in this document.
