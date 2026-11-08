# ☀️ Napelem ERP Fejlesztői Csoport (Helios ERP)

> Intelligens raktárlogisztikai és vállalatirányítási ökoszisztéma napelem-telepítési projektek koordinálására.

Üdvözlünk a szervezetünk GitHub oldalán! Csapatunk modern szoftvertechnológiai és minőségbiztosítási módszertanokat (CI/CD, Feature-Branch workflow, Clean Architecture, szálbiztos adatbázis-tranzakciók, automatizált integrációs tesztelés) alkalmazva fejleszti a **Napelem ERP (Helios ERP)** vállalatirányítási rendszert.

---

### 🚀 Központi Rendszerünk: [`Napelem-erp`](https://github.com/zek-gazdinfo-2025/Napelem-erp)

A szoftver egy robusztus, mikroszolgáltatás-alapú Python / FastAPI és SQLAdmin vállalati háttérmotor, amely teljes körűen lefedi a napelemes kivitelezések fizikai és üzleti folyamatait:

* 📦 **240 Rekeszes Raktárhálózat:** 3D koordináta-alapú fizikai tárolórendszer (`S1-O1-SZ1` – `S10-O4-SZ6`), rekeszszintű túlcsordulás- és keveredésvédelemmel, önürítő logikával és öngyógyító seederrel.
* ⚙️ **7 Fázisú Projekt-Életciklus:** Szigorú átmeneti mátrixszal védett állapotgép (State Machine), élő folyamatsáv (Pipeline) és időbélyeges, felhasználóhoz kötött eseménynapló (`ProjectStatusLog`) a felméréstől a zárásig.
* 🗺️ **Interaktív 2D Raktártérkép & Hőtérkép:** 6 szintes vertikális rétegválasztó, dinamikus szinttelítettségi mutató (`%`), cikk-kiemelő kereső és közvetlen kétirányú készletkezelés (Stock-in / Stock-out).
* 📋 **Raktári Komissiózás & Szedőív (C.1, C.2):** Tételes kiszedési lista fizikai koordinátákkal (`GET /projects/{id}/picking-list`), készletlevonás (`POST /projects/{id}/start-picking`), és hivatalos nyomtatható A4-es szedőív.
* 📍 **3D Legközelebbi Szomszéd Útvonaltervezés (C.3):** Komissiózási bejárási sorrend és gyaloglási távolság minimalizálása a 240 rekeszen keresztül (`GET /projects/{id}/optimized-route`).
* 📊 **Pénzügyi Kalkuláció & Árajánlat (A.6):** Anyagköltség, munkaórák és munkadíj elszámolása 27%-os ÁFA kalkulációval és nyomtatható A4-es hivatalos árajánlattal (`quote-sheet`).
* 🚚 **Beszállítói Hiánylista & Rendelés (B.3, B.4):** Az összes aktív projekt hiánycikkeinek gépi JSON összesítése és pecsételhető A4-es rendelési diszpozíció (`missing-parts-sheet`).
* 🔒 **Szerepkör-alapú Védelem (RBAC & JWT):** Bcrypt jelszótitkosítás, 60 perces JWT Bearer tokenek, munkamenet-alapú SQLAdmin autentikáció (`login.html`), valamint elkülönített feladatkörök (Admin, Szakember, Raktárvezető, Raktáros).
* 🛡️ **Hivatalos Projektzárás és Módosításvédelem (A.7):** Végállapotok zárolása (`Completed` / `Failed`), utólagos felülírások megakadályozása és főadminisztrátori önvédelem.

---

### 🛠️ Alkalmazott Technológiai Stack & Rendszerjelvények

![Python](https://img.shields.io/badge/Python-3.13-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-0.110+-009688?style=flat&logo=fastapi&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-ORM%202.0-D71F00?style=flat&logo=sqlalchemy&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-WAL%20Database-003B57?style=flat&logo=sqlite&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-v2-E92063?style=flat&logo=pydantic&logoColor=white)
![SQLAdmin](https://img.shields.io/badge/Admin-SQLAdmin-10B981?style=flat&logo=fastapi&logoColor=white)
![Pytest](https://img.shields.io/badge/Tests-30%2F30%20Passed-0A9EDC?style=flat&logo=pytest&logoColor=white)
![Docs](https://img.shields.io/badge/Docs-Swagger%20UI-85EA2D?style=flat&logo=swagger&logoColor=black)
[![Release](https://img.shields.io/badge/Release-v2.8.4-blue?style=flat)](https://github.com/zek-gazdinfo-2025/Napelem-erp/releases)
[![Render Live](https://img.shields.io/badge/Render-Live%20Demo-46E3B7?style=flat&logo=render&logoColor=white)](https://napelem-erp.onrender.com/admin/)
[![Swagger API](https://img.shields.io/badge/API-Swagger%20UI-85EA2D?style=flat&logo=swagger&logoColor=black)](https://napelem-erp.onrender.com/docs/)
[![CI Tests](https://github.com/zek-gazdinfo-2025/Napelem-erp/actions/workflows/tests.yml/badge.svg)](https://github.com/zek-gazdinfo-2025/Napelem-erp/actions) 

---

### 📌 Mérföldkő Státusz és Munkafolyamat

> 🚀 **Hivatalos Állapot: 1., 2. és 3. Mérföldkő funkciói lezárva és integrálva (`v2.8.4`)**  
> Az alaprendszer, a 240 rekeszes raktárlogisztika, a 7 fázisú projekt állapotgép, a 3D útvonaltervezés, az árajánlat- és hiánylista-kalkuláció, az RBAC jogosultságkezelés és a **30/30 integrációs teszt** sikeresen teljesítve.  
> 📍 **Jelenlegi fázis:** Záró felkészülés a tanszéki védésre, a hordozható bináris (`NapelemERP_v3.exe`) véglegesítése és a prezentációs főpróba.

* 📋 **[GitHub Projects Kanban Tábla](https://github.com/orgs/zek-gazdinfo-2025/projects/3)** – *Valós idejű sprint- és feladatkövetés.*
* 📦 **[Hivatalos Kiadások (Releases)](https://github.com/zek-gazdinfo-2025/Napelem-erp/releases)** – *Mérföldkő-csomagok és önálló futtatható binárisok (`.exe`).*
* 📚 **[Rendszertervek és Technikai Dokumentáció](https://github.com/zek-gazdinfo-2025/Napelem-erp/tree/master/docs)** – *Architektúra-döntések, állapotgép, feladatmegosztási mátrix és kockázatelemzés.*

---

### 🤝 Fejlesztési és Minőségbiztosítási Szabályaink

1. 🌿 **Feature-Branch Workflow:** A védett `master` ágra közvetlen feltöltés tilos; minden fejlesztési tétel külön `feature/<modul>` ágon készül.
2. 🧪 **Automatizált CI Védőháló:** Minden Push és Pull Request esetén GitHub Actions virtuális gépen lefut a **30 független integrációs tesztesetet** tartalmazó Pytest csomag.
3. 🔍 **Kódátnézés (Code Review):** Kód beolvasztása kizárólag zöld teszteredmény ($\checkmark$) és a Tech Lead jóváhagyása után történhet.
4. 📖 **Transzparens Rendszerterv:** Minden architekturális döntést, relációs sémát és üzleti szabályt verziókövetett dokumentumok rögzítenek a `docs/` könyvtárban.

---

📍 **Pannon Egyetem ZEK – Gazdaságinformatika (2025/2026)**  
*Szoftvertechnológia tantárgyi projektmunka*
