# ☀️ Napelem ERP Fejlesztői Csoport

> Intelligens raktárlogisztikai és vállalatirányítási ökoszisztéma napelem-telepítési projektek koordinálására.

Üdvözlünk a szervezetünk GitHub oldalán! Csapatunk modern szoftvertechnológiai módszertanokat (CI/CD, Feature-Branch workflow, Clean Architecture, automatizált integrációs tesztelés) alkalmazva fejleszti a **Napelem ERP** vállalatirányítási rendszert.

---

### 🚀 Központi Rendszerünk: [`Napelem-erp`](https://github.com/zek-gazdinfo-2025/Napelem-erp)

A szoftver egy robusztus Python / FastAPI mikroszolgáltatás-alapú háttérmotor, amely teljes körűen lefedi a napelemes kivitelezések fizikai és üzleti folyamatait:

* 📦 **240 Rekeszes Raktárhálózat:** 3D koordináta-alapú tárolás (`S1-O1-SZ1` – `S10-O4-SZ6`), rekeszszintű túlcsordulás- és keveredésvédelemmel, közvetlen kétirányú gyorsműveletekkel (Stock-in / Stock-out) és automatikus rekeszfelszabadítással.
* ⚙️ **7 Fázisú Projekt-Életciklus:** Szigorú érvényesítésű állapotgép (State Machine), folyamatsáv (Pipeline) és időbélyeges eseménynapló (`ProjectStatusLog`) a megrendeléstől az átadásig.
* 📋 **Raktári Kiszedés & Szedőív (C.1, C.2):** Tételes komissiózási jegyzék lokációkkal, azonnali készletlevonás és nyomtatható A4-es hivatalos kísérőlevél átadási aláírásokkal.
* 🔒 **Szerepkör-alapú Védelem (RBAC):** Sózott SHA-256 jelszóbiztonság, elkülönített feladatkörök (Adminisztrátor, Szakember, Raktárvezető, Raktáros).
* 🖥️ **Adminisztrációs és Térkép Felület:** Böngészős SQLAdmin felület (`/admin`), interaktív 2D raktártérkép szintes telítettségi mutatókkal és Swagger UI (`/docs`).
* 📊 **Pénzügyi Kalkuláció & Beszerzés:** Tételes anyagköltség- és munkadíjszámítás, 27%-os ÁFA kalkuláció és hiánycikk-összesítés.

---

### 🛠️ Alkalmazott Technológiai Stack

![Python](https://img.shields.io/badge/Python-3.13-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-0.110+-009688?style=flat&logo=fastapi&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-ORM-D71F00?style=flat&logo=sqlalchemy&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-Database-003B57?style=flat&logo=sqlite&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-v2-E92063?style=flat&logo=pydantic&logoColor=white)
![SQLAdmin](https://img.shields.io/badge/Admin-SQLAdmin-10B981?style=flat&logo=fastapi&logoColor=white)
![Pytest](https://img.shields.io/badge/Tests-Pytest-0A9EDC?style=flat&logo=pytest&logoColor=white)
![Docs](https://img.shields.io/badge/Docs-Swagger%20UI-85EA2D?style=flat&logo=swagger&logoColor=black)
[![Release](https://img.shields.io/badge/Release-v2.5.1-blue?style=flat)](https://github.com/zek-gazdinfo-2025/Napelem-erp/releases/tag/v2.5.1)
[![Render Live](https://img.shields.io/badge/Render-Live%20Demo-46E3B7?style=flat&logo=render&logoColor=white)](https://napelem-erp.onrender.com/admin/)
[![Swagger API](https://img.shields.io/badge/API-Swagger%20UI-85EA2D?style=flat&logo=swagger&logoColor=black)](https://napelem-erp.onrender.com/docs/)
[![CI Tests](https://github.com/zek-gazdinfo-2025/Napelem-erp/actions/workflows/tests.yml/badge.svg)](https://github.com/zek-gazdinfo-2025/Napelem-erp/actions) 

---

### 📌 Mérföldkő Státusz és Munkafolyamat

> 🚀 **Hivatalos Állapot: 1. & 2. Mérföldkő lezárva, 3. Mérföldkő folyamatban (`v2.5.1`)**  
> Az alaparchitektúra, a 240 rekesz kétirányú logisztikai motorja, az SQLAdmin felület, a raktári kiszedési folyamat (C.1, C.2) és a 16/16 integrációs teszt sikeresen teljesítve.  
> 📍 **Jelenlegi fázis:** A 3. Mérföldkő csapatfeladatainak (optimális útvonaltervezés, RBAC végpontvédelem, pénzügyi kalkuláció és projektzárás) integrációja.

* 📋 **[GitHub Projects Kanban Tábla](https://github.com/orgs/zek-gazdinfo-2025/projects/3)** – *Valós idejű sprint- és feladatkövetés.*
* 📦 **[Hivatalos Kiadások (Releases)](https://github.com/zek-gazdinfo-2025/Napelem-erp/releases)** – *Mérföldkő-csomagok és önálló futtatható binárisok (`.exe`).*
* 📚 **[Rendszertervek és Technikai Dokumentáció](https://github.com/zek-gazdinfo-2025/Napelem-erp/tree/master/docs)** – *Architektúra-döntések, állapotgép és feladatkiosztás.*

---

### 🤝 Fejlesztési és Minőségbiztosítási Szabályaink

1. 🌿 **Feature-Branch Workflow:** A védett `master` ágra közvetlen feltöltés tilos; minden feladat külön `feature/<modul>` ágon készül.
2. 🧪 **Automatizált CI Védőháló:** Minden Push és Pull Request esetén GitHub Actions virtuális gépen automatikusan lefut a 16 tesztesetet tartalmazó Pytest tesztcsomag.
3. 🔍 **Kódátnézés (Code Review):** Kód beolvasztása kizárólag zöld teszteredmény és a Tech Lead jóváhagyása után történhet.
4. 📖 **Transzparens Rendszerterv:** Minden architekturális döntést és üzleti szabályt verziókövetett dokumentumok rögzítenek a `docs/` mappában.

---

📍 **Pannon Egyetem ZEK – Gazdaságinformatika**  
*Szoftvertechnológia tantárgyi projektmunka*
