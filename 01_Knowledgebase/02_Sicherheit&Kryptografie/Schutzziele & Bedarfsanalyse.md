
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
|                  |                                                                                                                                                                                               |
| ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Methode**      | Kryptografie                                                                                                                                                                                  |
| **Technologien** | Verschlüsselung & Hashing                                                                                                                                                                     |
| **Schutzziele**  | Vertraulichkeit, Integrität, Authentizität, Verbindlichkeit                                                                                                                                   |
| **Beschreibung** | Der Einsatz von Algorithmen, um Daten unlesbar zu machen (schützt _Vertraulichkeit_) oder um Prüfsummen zu bilden, die Manipulationen aufdecken (schützt _Integrität_ und _Verbindlichkeit_). |

|                  |                                                                |
| ---------------- | -------------------------------------------------------------- |
| **Methode**      | Identitäts- und Zugriffsmanagement                             |
| **Technologien** | User Accounts, Multi-Faktor-Authentifizierung                  |
| **Schutzziele**  | Vertraulichkeit, Integrität, Authentizität, Verbindlichkeit    |
| **Beschreibung** | Systeme, die sicherstellen, dass sich Nutzer ausweisen müssen. |

|                  |                                                                            |
| ---------------- | -------------------------------------------------------------------------- |
| **Methode**      | Endgerätesicherheit                                                        |
| **Technologien** | Antiviren-Software, Endpoint Detection and Response                        |
| **Schutzziele**  | Vertraulichkeit, Integrität, Verfügbarkeit, Authentizität, Verbindlichkeit |
| **Beschreibung** | Durch das Verhindern, Erkennen und Isolieren von Schadsoftware können Dinge wie Daten-leaks, Ausfälle und  Identity hijacking verhindert werden. |

|                  |                                                                            |
| ---------------- | -------------------------------------------------------------------------- |
| **Methode**      | Backups & Redundanzen                                                        |
| **Technologien** | Antiviren-Software, Endpoint Detection and Response                        |
| **Schutzziele**  | Integrität, Verfügbarkeit |
| **Beschreibung** |              |
