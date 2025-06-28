# 🔷 Power BI Roadmap für ITIL-Initiativen 🔷

Diese Lösung stellt eine vollständig automatisierte Power BI Roadmap zur Verfügung – mit tagesgenauer Phasenverfolgung, KPI-Messung und Reifegradbewertung. Ideal für ITIL-Programme, Sprint-Steuerung, Transformationstracking oder Reifegradmanagement.

---

##  Zielsetzung

✔️ Visualisierung von **ITIL-Projektphasen auf Tagesbasis**  
✔️ Transparente Darstellung von **Reifegrad, Risiko und Status**  
✔️ Automatisierte Erstellung von **Gantt-ähnlichen Zeitachsen** 
✔️ Unterstützung für **Daily Standups, Sprintplanung und Governance-Berichte**

---

##  Architekturkomponenten

### Measures & Berechnungen

| Measure                    | Zweck |
|----------------------------|-------|
| `AktivePhasen_Heute`       | Zählt aktuelle Tagesphasen (Roadmap KPI) |
| `Anzahl_PhaseGeplant`      | Anzahl aller Projektphasen im Modell |
| `Heute_Linie`              | Visualer Marker für heutiges Datum in Diagrammen |
| `PhAktiv_Tage`             | Zählt alle aktiven Phasentage |

---

## Berechnete Spalten & Tabellen

| Element              | Beschreibung |
|----------------------|--------------|
| `DatumsTabelle`      | Zeitdimension für 2023–2026 mit Formatierungen |
| `Roadmap_Tage`       | Gantt-Linienstruktur – pro Phase ein Tagesabschnitt |
| `Dauer_Tage`         | Differenz in Tagen zwischen Start- und Enddatum |
| `Offset_Start`       | Horizontale Verschiebung für Balkendiagramme |
| `Startdatum_Date`    | Text zu Datum Konvertierung (mit Wochentags-Korrektur) |
| `Doku_KPI`           | Kommentar-/Dokutabelle für Metadaten und Kontextinfos |

---

## Projektstruktur

```bash
Power_BI_Roadmap/
├── AktivePhasen_Heute.dax
├── Anzahl_PhaseGeplant.dax
├── DatumsTabelle.dax
├── Dauer_Tage.dax
├── Doku_KPI.dax
├── Enddatum_Date.dax
├── Fortschritt_Prozent.dax
├── Heute_Linie.dax
├── Offset_Start.dax
├── PhAktiv_Tage.dax
├── Roadmap_Tage.dax
├── Startdatum_Date.dax
└── README.md
```
---

##  Verwandte Repositorien

-  **ITIL-Practice-Governance-Bebauungsplan**: (https://github.com/Dofp79/ITIL-Practice-Governance-Bebauungsplan)
-  **ITSM_Power_BI_Vorlage_1.0.0**: (https://github.com/Dofp79/ITSM_Power_BI_Vorlage_1.0.0)
-  **Referatskapazität – Analysemodell für Sprint- & Teamkapazitäten in Power BI**: (https://github.com/Dofp79/Referatskapazit-t/tree/main)

---

## 📫 Kontakt

Fragen oder Feedback?  
**Doniman F. Peña Parra**

- 🌐 [GPT-Link zur Projektunterstützung](https://chatgpt.com/g/g-68150f83fda081919d979c8418039ee5-dashboard-design)  
- 🔗 [LinkedIn](https://www.linkedin.com/in/doniman-francisco-pe%C3%B1a-parra-609263232/)  
- ✉️ [dofp79@hotmail.com](mailto:dofp79@hotmail.com)

---
