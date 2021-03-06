---
title: Formatbeispiel für den Import von Produktdaten
layout: default
tags:
  - Datenverwaltung
  - Datenimport
  - Produktdatenimport
lang: de
sequence: 10
ref: import_format_example_product
---

## Überblick
Für den Produktdatenimport benötigst Du ein Importformat, in dem die **DB-Tabelle** *Import - Produkt* eingestellt ist.

In dem folgenden Beispiel wird der Dateninhalt aus einer Datei einer Tabellenkalkulationssoftware (hier z.B. eine *Excel*-Datei vor der [Konvertierung in eine CSV- oder TXT-Datei](Importdatei_nuetzliche_Hinweise)) dem Importformat für Produktdaten gegenübergestellt:

![](assets/Produktimport_Excel-Tabelle_Format.png)

### Erläuterungen zum Beispiel
- Die **Spalte A** der Excel-Tabelle (*Artikelnummer*) steht an erster Stelle, d.h. das entsprechende Formatfeld bekommt die **Start-Nr. 1**. Demzufolge erhält das Formatfeld für die **Spalte B** die **Start-Nr. 2** usw.<br> Die **Reihenfolge** der Formatfelder ist dabei unerheblich.
 >**Hinweis:** metasfresh erwartet ***keine Spaltennamen*** in der Importdatei. Alleine die ***Position*** der Spalte muss mit der Startnummer übereinstimmmen.

- Der **Name** des Formatfeldes ist frei wählbar und muss nicht mit der Benennung der Spalte aus der Importdatei übereinstimmen.
- Die **Spalte** des Formatfeldes bestimmt, wohin metasfresh den Inhalt der Spalte aus der Importdatei übertragen soll.
- Der **Datentyp** bestimmt, ob es sich bei den Importdaten z.B. um eine *Zeichenfolge* oder *Zahl* handelt.

### Einige nützliche Hinweise
Die Angabe der Pflichtfelder ist unerlässlich für einen erfolgreichen Datenimport!

| Pflichtfeld | <abbr title="Bewege den Mauszeiger über den Feldnamen, um den entspr. Spaltennamen zu sehen.">Feldname</abbr> | Beispiel | Hinweis |
| :---: | :---: | :--- | :--- |
| X | <abbr title="Value_Suchschlüssel">Artikelnummer</abbr> | FF_12345 | **Suchschlüssel** des Produktes (alphanumerische Zeichenfolge) |
| X | <abbr title="ProductType_Produktart">Produktart</abbr> | I | I = Artikel (engl.: _**I**tem_)<br> E = **E**rfolgskonten<br> R = **R**essource |
| X | <abbr title="ProductCategory_Value_Produktkategorie-Schlüssel">Produktkategorie-Schlüssel</abbr> | •&nbsp;Diverse<br> •&nbsp;16 | **Suchschlüssel** der Produktkategorie.<br> ***Achtung:*** Nicht der Name!<br> (*Den Suchschlüssel kannst Du unter dem Menüpunkt "[Produkt Kategorie](Menu)" nachschauen.*) |
|  | <abbr title="X12DE355_Kodierung der Mengeneinheit">Kodierung der Mengeneinheit</abbr>	| PCE | PCE = Stück (Stk, engl.: _**P**ie**ce**_)<br> (*Die Kodierungen der Mengeneinheiten kannst Du unter dem Menüpunkt "[Maßeinheit](Menu)" nachschauen.*) |
|  | <abbr title="C_TaxCategory_Name_MwSt-Kategorie">MwSt-Kategorie</abbr> | Reduzierter Steuersatz 7% (Deutschland) | Die MwSt-Kategorie kannst Du unter dem Menüpunkt "[Steuer Kategorie](Menu)" nachschauen. |
|  | <abbr title="M_PriceList_Version_Name_Version Preisliste">Version Preisliste</abbr> | Testpreise Kunden (Deutschland) | Die Preislistenversion kannst Du unter dem Menüpunkt "[Preisliste](Menu)" nachschauen. |

## Nächste Schritte
- [Produktdaten importieren](Produktdaten_importieren).
