
> [!abstract] Ziel
> Mit einer Schutzbedarfsanalyse kann das Sicherheitsniveau von Informationssystemen bewertet werden. Damit können potentielle Risiken erkannt und bewertet werden um anschließend entsprechende Sicherheitsmaßnahmen zu priorisieren. Ultimatives Ziel ist, für die verarbeiteten Informationen einen angemessen Schutz sicherzustellen.

# Schutzziele
Grundsätzlich lassen sich drei allgemeine Schutzziele definieren:
- **Vertraulichkeit** (confidentiality): Nur autorisierte Benutzer und Dienste dürfen auf Daten zugreifen. Das gilt bei gespeicherten, als auch bei übertragenen Daten.
- **Integrität** (integrity): Daten dürfen nicht unbemerkt verändert werden. Änderungen müssen nachvollziehbar sein.
- **Verfügbarkeit** (availability): Der Zugriff auf Daten muss gewährt werden, Systemausfälle verhindert.

Da die grundsätzlichen Schutzziele nicht alle Bedarfe abdecken, wurden weitere Ziele definiert, unter Anderem:
- **Authentizität** (authenticity):
	- Entitäten: Ist z.B. die Person auch die für die sie sich ausgibt?
	- Daten: Stammt z.B. die E-Mail wirklich von dem angegebenen Postfach?
- **Verbindlichkeit** (non repudiation): Übertragene Daten sind verbindlich und damit nachvollziehbar. z.B. Eine E-Mail ist Verbindlich beim Empfänger angekommen und kann nachgewiesen werden.

# Methoden
- [[Verschluesselung_Sym_Asym|Kryptografie]]
	- **Technologien**: Verschlüsselung & Hashing
	- **Schutzziele**: Vertraulichkeit, Integrität, Authentizität, Verbindlichkeit
	- **Beschreibung**: Der Einsatz von Algorithmen, um Daten unlesbar zu machen (schützt _Vertraulichkeit_) oder um Prüfsummen zu bilden, die Manipulationen aufdecken (schützt _Integrität_ und _Verbindlichkeit_).
- Identitäts- und Zugriffsmanagement
	- **Technologien**: User Accounts, Multi-Faktor-Authentifizierung
	- **Schutzziele**: Vertraulichkeit, Integrität, Authentizität, Verbindlichkeit
	- **Beschreibung**: Systeme, die sicherstellen, dass sich Nutzer ausweisen müssen.
- Endgerätesicherheit
	- **Technologien**: Antiviren-Software, Endpoint Detection and Response
	- **Schutzziele**: Vertraulichkeit, Integrität, Verfügbarkeit, Authentizität, Verbindlichkeit
	- **Beschreibung**: Durch das Verhindern, Erkennen und Isolieren von Schadsoftware können Dinge wie Daten-leaks, Ausfälle und  Identity hijacking verhindert werden.
- Backups & Redundanzen
	- **Technologien**: gespiegelte Drives, Kopien auf Tapes, doppelte Bereitstellung von Hardware
	- **Schutzziele**: Integrität, Verfügbarkeit
	- **Beschreibung**: Durch gespiegelte Daten können Integritäts-Checks durchgeführt werden, durch Redundanzen Ausfälle verhindert.

Auch Dinge wie Zutrittskontrollen, Schulungen der Mitarbeitenden, Rechtekonzepte, Umgebungsschutz (Klimaanlagen, Feuerlöschsysteme, usw.) und sichere Entsorgung von Datenträgern sind Methoden, um einen Schutzbedarf zu erfüllen.

---

# Prüfungsaufgaben
## Schutzziele
### Szenario Zeiterfassung
[[Sommer 2023 FISI Analyse.pdf|Sommer 2023 Analyse]]
**Aufgabe 1.2.1** Erläutern Sie den notwendigen Schutzbedarf von zu erfassenden Daten in Bezug auf die Zeiterfassung der AntiCov AG anhand von zwei unterschiedlichen Schutzzielen.

> [!check]- Lösung
> [[Sommer 2023 FISI Analyse - Lösung.pdf|Sommer 2023 Analyse - Lösung]]
> 1. *Vertraulichkeit:* Daten (Namen, Arbeitszeiten) dürfen nur von berechtigten Personen (Vorgesetzte, Personalabteilung) eingesehen werden
> 2. *Integrität:* Nur Befugte dürfen Daten verändern, um Fehlbuchungen oder Manipulationen zu verhindern. **Verfügbarkeit:** Die Erfassung muss reibungslos funktionieren, um Fehlerquellen bei Systemausfällen zu minimieren.

---

### Szenario Schulnetzwerk
[[Sommer 2023 FISI Konzeption.pdf|Sommer 2023 Konzeption]]
**Aufgabe 1.4.1** Erläutern Sie in Bezug auf die unterschiedlichen Netze der Schule die folgenden Begriffe und nennen Sie je ein Beispiel: 
- Integrität
- Vertraulichkeit
- Authentizität

> [!check]- Lösung 
> [[Sommer 2023 FISI Konzeption -  Lösung.pdf|Sommer 2023 Konzeption -  Lösung]]
> - **Vertraulichkeit:** Informationen (z. B. Schülerarbeiten) sind nur Befugten zugänglich
> - **Integrität:** Es besteht keine Möglichkeit der unbefugten Datenmanipulation (z. B. verschlüsselter Abruf von Daten).
> - **Authentizität:** Identitätsnachweis des Kommunikationspartners (z. B. Login mit Benutzername und Passwort).

---

### Szenario VPN 
[[Winter 2023 FISI Konzeption Aufgaben.pdf|Winter 2023 Konzeption]]
**Aufgabe 1.4.2** Erläutern Sie die Anforderungen an ein [[VPN_SiteToSite_Remote|VPN]] hinsichtlich der drei Schutzziele.

> [!check]- Lösung 
> [[Winter 2023 FISI Konzeption - Lösung.pdf|Winter 2023 Konzeption - Lösung]]
> - *Authentizität:* Der Partner ist wirklich der, der er vorgibt zu sein (z. B. Zertifikate)
> - *Integrität:* Korrektheit der Daten; Veränderungen bleiben nie unentdeckt (z. B. Hash).
> - *Vertraulichkeit:* Daten sind nur für die Kommunikationspartner einsehbar (z. B. Verschlüsselung).

---

## Aufgaben zur Schutzbedarfs- und Risikoanalyse

### Analyse von Netzkomponenten 
[[Sommer 2023 FISI Analyse.pdf|Sommer 2023 Analyse]]
Aufgabe 1.3.1: Analysieren Sie den Netzwerkplan in Anlage 1. Geben Sie an, welche verschiedene Komponenten erhöhten Schutzbedarf haben und begründen Sie Ihre Entscheidung.

> [!example]- Anlage 1
> ![[Sommer_2023_Analyse_Anlage1.png]]

> [!check]- Lösung
> [[Sommer 2023 FISI Analyse - Lösung.pdf|Sommer 2023 Analyse - Lösung]]
>Die **Firewall (N1)** muss immer verfügbar sein und darf nur zulässige Infos weiterleiten (Integrität). **Switches (N2-N4)** müssen verfügbar sein, um das Netz funktionstüchtig zu halten. Auf **Virtualisierungsserver (S1)** und **DBMS (S5)** liegen alle Mitarbeiterdaten, die nur von Berechtigten aufgerufen werden dürfen.

---

### Risikoeinstufung
[[Sommer 2023 FISI Analyse.pdf|Sommer 2023 FISI Analyse]]
**Aufgabe 1.3.3** Führen Sie für folgende Komponenten eine Risikoeinstufung (Anlage 3 und 4) mit ausführlicher Begründung durch:
- Virtualisierungsserver S1 am Beispiel des Wartungsvorgangs (Gefährdungen: Abhören und Ausfall von Geräten oder Systemen)
- Datenbankmanagementsystem A1 am Beispiel der Stundenerfassung (Gefährdungen: Software- Schwachstellen oder -Fehler und Gefährdung, sowie Missbrauch von Berechtigungen)

> [!example]- Anlage 3 & 4
> ![[Sommer_2023_Analyse_Anlage3.png]]
> ![[Sommer_2023_Analyse_Anlage4.png]]

> [!check]- Lösung
> [[Sommer 2023 FISI Analyse - Lösung.pdf|Sommer 2023 Analyse - Lösung]]
> Durch fehlende Verschlüsselung kann beim Verschieben von VMs der Datenstrom mitgelesen werden. Dies verletzt Vertraulichkeit und Integrität stark und kann für eine Firma existenzbedrohend sein.

---

## Sicherheitsprinzipien
[[Sommer 2025 FISI Konzeption und Administration IT-Systeme.pdf]]
**Aufgabe 2 e)** Sicherheitsexperten empfehlen im Rahmen von Sicherheitskonzepten für IT-Systeme folgende Prinzipien: Das Least-Privilege-Prinzip und das Zero-Trust-Prinzip. Beide Prinzipien sollen bei der Retailer GmbH implementiert werden. Erläutern Sie zu jedem Prinzip eine typische Maßnahme.

> [!check]- Lösung 
> [[Sommer 2025 FISI Konzeption - Lösung.pdf]]
> **Least-Privilege:** Personen erhalten nur die Rechte, die für die Erledigung der Aufgaben zwingend erforderlich sind, um Missbrauch zu verhindern
> **Zero-Trust:** Ständige Überwachung des Zugriffs der Systeme untereinander innerhalb des Firmennetzes, um die Ausbreitung von Schadsoftware zu verhindern.

---

# Verknüpfungen

**Zur Umsetzung von Vertraulichkeit (Confidentiality):**
- [[Verschluesselung_Sym_Asym]] (Wie mache ich Daten unlesbar?)
- [[VPN_SiteToSite_Remote]] (Wie schütze ich Daten bei der Übertragung?)
- [[Identitaetsmanagement_MFA]] (Wie stelle ich sicher, dass nur Befugte zugreifen?)
- [[Firewall_Arten_Regelwerke]] (Wie sperre ich Unbefugte aus dem Netz aus?)

**Zur Umsetzung von Integrität (Integrity):**
- [[Hashing_und_Salting]] (Wie prüfe ich, ob eine Datei verändert wurde?)
- [[Digitale_Zertifikate_PKI]] (Wie beweise ich die Echtheit eines Senders?)

**Zur Umsetzung von Verfügbarkeit (Availability):**
- [[Backup_Strategien]] (Wie stelle ich Daten nach einem Ausfall wieder her?)
- [[Storage_RAID_Level]] (Wie schütze ich mich vor Festplattenausfällen?)
- [[USV]] (Wie überbrücke ich Stromausfälle?)
- [[Netzwerk_Redundanz_STP_HSRP]] (Wie verhindere ich Netzwerkausfälle?)
