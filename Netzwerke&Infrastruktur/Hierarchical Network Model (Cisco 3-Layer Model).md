> [!abstract] Definition
> 
> Ein strukturelles Design-Modell für Unternehmensnetzwerke, das die Komplexität reduziert, die Skalierbarkeit erhöht und die Fehlersuche vereinfacht. Es teilt das Netzwerk in drei spezialisierte Schichten (Layer) auf.

## Layers

### 1. Access Layer (Zugangsschicht)

- **Aufgabe:** Verbindet Endgeräte (PCs, Drucker, APs) mit dem Netzwerk.
    
- **Funktionen:**
    
    - Layer-2-Switching.
        
    - **Port-Security** (MAC-Filterung).
        
    - VLAN-Zuweisung.
        
    - PoE (Power over Ethernet) für Telefone/Kameras.
        
    - ARP-Inspection & DHCP Snooping.
        
- **Hardware:** Kostengünstige Switches mit hoher Portdichte.
    

### 2. Distribution Layer (Verteilungsschicht)

- **Aufgabe:** Verbindung zwischen Access- und Core-Layer; Aggregation der Access-Switches.
    
- **Funktionen:**
    
    - **Inter-VLAN-Routing** (Layer 3).
        
    - Anwendung von **ACLs** (Security Policies & Paketfilterung).
        
    - Routing zwischen Subnetzen.
        
    - Redundanz-Protokolle (z. B. HSRP/VRRP).
        
    - Definition von Broadcast-Domänen.
        
- **Hardware:** Layer-3-Switches oder Router.
    

### 3. Core Layer (Backbone)

- **Aufgabe:** Hochgeschwindigkeits-Transport zwischen den Distribution-Blöcken.
    
- **Funktionen:**
    
    - Maximaler Durchsatz und minimale Latenz.
        
    - **KEINE** Paketmanipulation (keine ACLs oder CPU-intensives Filtering).
        
    - Hochverfügbarkeit und Redundanz.
        
- **Hardware:** High-End-Chassis-Switches mit enormer Backplane-Kapazität.

![[Cisco 3-Layer Model.png]]
Beispielaufbau eines Hierarchical Network Models

---

## Sonderform: Collapsed Core

In kleineren Netzwerken werden die Funktionen von **Core** und **Distribution** oft in einer Hardware-Schicht zusammengefasst, um Kosten zu sparen.

---

## Vorteile des hierarchischen Designs

|**Vorteil**|**Beschreibung**|
|---|---|
|**Skalierbarkeit**|Neue Netzwerkbereiche können einfach hinzugefügt werden, ohne den Core zu stören.|
|**Redundanz**|Durch doppelte Wege zwischen den Schichten (High Availability).|
|**Performance**|Core-Layer wird nicht durch Endgeräte-Traffic belastet.|
|**Einfache Wartung**|Fehler im Access-Layer bleiben lokal begrenzt.|

---

## Prüfungsrelevante Fragen (AP2-Check)

- [ ] Warum sollten ACLs im Distribution-Layer und nicht im Core-Layer platziert werden? (Antwort: Um den schnellen Durchsatz im Core nicht durch Rechenlast zu bremsen).
    
- [ ] Welche Geräte gehören typischerweise in den Access-Layer?
    
- [ ] Erkläre den Begriff "Stichleitung" oder "Uplink" im Kontext der Aggregation.
    

## 🔗 Verknüpfungen

- [[OSI-Modell]]
    
- [[VLAN-Konfiguration]]
    
- [[Inter-VLAN-Routing]]
    
- [[Netzwerk-Redundanz-HSRP]]
    

#Netzwerktechnik #AP2 #Infrastruktur #Cisco
