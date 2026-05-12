> [!abstract] Definition
> Ereignisgesteuerte Prozessketten sind graphische Darstellungen von Prozessen in einer Organisation. Diese besteht primär aus Ereignissen, Funktionen und Konnektoren. Bei der erweiterten Ereignisgesteuerten Prozesskette (eEPK) werden zusätzlich Informationsobjekte und Organisationseinheiten angegeben.

# Symbole & Knoten
## Ereignis 
Ein Ereignis ist ein Zustand, der vor oder nach einer Funktion auftritt. Das Symbol ist ein gestrecktes Rechteck. Beispiel: "Auftrag ist angekommen." 

![Ereignis](EPK_Ereignis.png)

## Funktion 
Eine Funktion ist eine Aktion oder eine Aufgabe, auf die ein Ereignis folgt. Das Symbol ist ein Rechteck mit abgerundeten Kanten. Beispiel: "Auftrag prüfen"

![Funktion](EPK_Funktion.png)

## Konnektoren 
Konnektoren sind Logikgatter, die genutzt werden um den Kontrollfluss aufzuteilen. Verfügbare Konnektoren sind UND, ODER und XOR (Exklusiv-ODER). Das Symbol ist ein Kreis mit dem entsprechenden Symbol. 

| UND                 | ODER                  | XOR                 |
| ------------------- | --------------------- | ------------------- |
| ![UND](EPK_UND.png) | ![ODER](EPK_ODER.png) | ![XOR](EPK_XOR.png) |

## Organisationseinheit (OE)
Mit Organisationseinheiten werden Rollen oder Abteilungen dargestellt. Niemals aber werden Personen oder Stellen namentlich erwähnt. Das Symbol ist eine Ellipse, die vor dem linken Rand eine senkrechte Linie enthält. Beispiel: "Marketingabteilung" 

![Organisationseinheit](EPK_Organisationseinheit.png)

## Informationsobjekt (IO) 
Eine Informationsobjekt stellt Dokumente oder andere Datenspeicher dar (z.B. Datenbanken). Das Symbol ist ein Rechteck. Beispiel: "Kundendatenbank" 

![Informationsobjekt](EPK_Informationsobjekt.png)

## Prozesswegweiser
Prozesswegweiser sind Hinweise auf andere Prozesse. Das Symbol ist ein Rechteck, hinter dem sich ein Sechseck verbirgt.

![Prozesswegweiser](EPK_Prozesswegweiser.png)

# Syntax 
- Gelesen wird von oben nach unten
- Beginn und Ende ist immer ein Ereignis
- Organisationseinheiten und Informationsobjekte sind Symbole der eEPK
- Der Informationsfluss wird durch Pfeile dargestellt
- Ereignisse und Funktionen haben jeweils einen Ein- und Ausgang
- Ausnahme: Anfangsereignis (kein Eingang), Endereignis (kein Ausgang)
- Treffen mehrere Ereignisse auf eine Funktion, sind Konnektoren nötig
- Ereignisse sind passiv, daher keine OR-/XOR-Aufspaltung zu mehreren Funktionen

> [!example]- Beispiel
> ![image](prozessablaufEPK.png)

---

# Verknüpfungen
## Tags
#ePK #Prozessmodellierung #Projektmanagement #Wirtschaft #Diagramme #LF12b #Knowledgebase