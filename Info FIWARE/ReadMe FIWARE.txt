===================================================================================================
FiwareSummit

Project:
https://app.asana.com/0/1204285422260806/1204530723943675/
https://github.com/msgis/arcgis-fiware.git

Author:
mailto:roman.trojan@msgis.com
Time:
[0141] Fiware.Summit _ms.GIS.Intern PRJ.Fiware_Summit

===================================================================================================

---------------------------------------------------------------------------------------------------
Entity-Types
---------------------------------------------------------------------------------------------------
Die Daten werden als JSON-Objekt aus Rest-Api �bernommen.
Alternativ k�nnten die Daten �ber JSON-File transferiert werden.

---------------------------------------------------------------------------------------------------
APRX
---------------------------------------------------------------------------------------------------
APRX muss "Fiware" und "Summit" im Dateinamen beinhalten.
z.B. "RT Wien Fiware_Summit.aprx"
Map muss den Tag "Fiware_Summit" beinhalten.
Map muss einen Layer mit Tag "Entities_Points" und Typ Point beinhalten.

---------------------------------------------------------------------------------------------------
AddInX
---------------------------------------------------------------------------------------------------
AddInX "msGIS.ProApp_FiwareSummit.esriAddinX" installieren.
(doppelklicken, aus ArcPro oder per GUID)
Sollte in folgendem Ordner ersichtlich sein:
C:\Users\[user]\Documents\ArcGIS\AddIns\ArcGISPro
Nach einem Start in ArcPro sollten die Komponenten ersichtlich werden:
C:\Users\[user]\AppData\Local\ESRI\ArcGISPro\AssemblyCache

---------------------------------------------------------------------------------------------------
ArcPro
---------------------------------------------------------------------------------------------------
ArcPro starten.
(aprx doppelklicken oder ArcGISPro.exe und aprx ausw�hlen)
Wenn alles korrekt abl�uft m�sste sich im Ribbon rechts eine Tab "FiwareSummit" zeigen.
Tab "FiwareSummit" klicken, es m�sste sich die Gruppe "FiwareSummit" mit weiteren Controls zeigen.
Button "Info FiwareSummit" ist nur informativ.
Button "Entity Types" klicken, es m�sste sich rechts eine Dockpane "FiwareSummit-Board" zeigen.

Nun kann per ComboBox "Entity type" ausgew�hlt werden.
Mit Klick auf Button "Entities zeigen" werden laut ausgew�hltem Typ die Entities per REST-Api
in ein JArray geladen und zu einem vordefinierten Layer hinzugef�gt.
Alle zuvor vorhandenen Objekte am Layer werden gel�scht.

(Stand 2023.05.26 Version 3.3.03)

W�nschenswert:
Layer Objekte mit Attribut "Typ" versehen, damit nur die entsprechenden Objekte gel�scht werden und auch sp�ter besser identifiziert werden k�nnen.
L�schen der Objekte entsprechend "Typ".
L�schen aller Objekte (Reset).
Dynamischer Update anhand per REST-Api. 
