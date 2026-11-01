# Portfolio — DTCSync — agente Windows com autoatualização

> Public case study only. **No source code** is published here (client/production systems remain private).  
> Estudo de caso público. **Sem código-fonte** (sistemas de cliente/produção permanecem privados).  
> Caso de estudio público. **Sin código fuente** (sistemas de cliente/producción permanecen privados).

---

## 🇧🇷 Português

### DTCSync — agente Windows com autoatualização

**Role / Papel / Rol:** Desenvolvimento completo (desktop + web local + empacotamento)  
**Stack:** `Python, HTML/CSS, PyInstaller, GitHub Releases, Windows services`

#### Problem / Problema
Clientes em campo precisavam de um agente Windows que se atualizasse sozinho, sem instalação manual a cada release, e com configuração simples via navegador.

#### Solution / Solução / Solución
Construí um executável Python com verificação de versão via GitHub Releases, troca segura do binário e reinício automático. Incluí painel web local para onboarding do cliente e rotação de logs.

#### Highlights
- Autoatualização a partir de releases
- Múltiplas instâncias no mesmo PC (portas distintas)
- Painel web local de configuração
- Empacotamento Windows (exe)


---

## 🇬🇧 English

### DTCSync — Windows agent with auto-update

**Role / Papel / Rol:** Full development (desktop + local web + packaging)  
**Stack:** `Python, HTML/CSS, PyInstaller, GitHub Releases, Windows services`

#### Problem / Problema
Field customers needed a Windows agent that could update itself without manual installs, with simple browser-based setup.

#### Solution / Solução / Solución
I built a Python executable that checks GitHub Releases, safely replaces the binary, and restarts. A local web panel handles client onboarding and log rotation.

#### Highlights
- Auto-update from releases
- Multiple instances on one PC (different ports)
- Local web configuration panel
- Windows packaging (exe)


---

## 🇪🇸 Español

### DTCSync — agente Windows con autoactualización

**Role / Papel / Rol:** Desarrollo completo (desktop + web local + empaquetado)  
**Stack:** `Python, HTML/CSS, PyInstaller, GitHub Releases, Windows services`

#### Problem / Problema
Los clientes en campo necesitaban un agente Windows que se actualizara solo, sin instalación manual, y con configuración simple por navegador.

#### Solution / Solução / Solución
Construí un ejecutable Python que consulta GitHub Releases, reemplaza el binario de forma segura y reinicia. Un panel web local cubre el onboarding y la rotación de logs.

#### Highlights
- Autoactualización desde releases
- Varias instancias en el mismo PC
- Panel web local de configuración
- Empaquetado Windows (exe)


---

## Notes / Observações / Notas

- Author: **Douglas Francisco Bonfim**
- Related private implementation (not public): `dtcsync`
- No credentials, customer data, hostnames, or proprietary payloads are included in this document.
