<div id="top"></div>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/cpro-iot">
    <img src="https://cpro-karriere.com/image/LOGO/doefwYl1s92eauMm83CoxrkXnOM76tazOd1RDgVzXeyn6h" alt="Logo" width="180" height="80">
  </a>
  
<h3 align="center">HBBK Münster: AR mit Vuforia Studio - Schulungsprojekt</h3>

  <p align="center">
  Zusammenfassung der wichtigsten Funktionen in Vuforia Studio mithilfe des Demoprojektes "Biegevorrichtung"
</div>

## Verzeichnis
- [Über das Projekt](#über-das-projekt)
  - [Entwickelt mit](#entwickelt-mit)
- [Getting Started](#getting-started)
  - [Voraussetzungen](#voraussetzungen)
  - [Installation](#installation)
  - [Grundfunktionen](#grundfunktionen)
  - [Javascript](#javascript)
- [Demoprojekt - "Biegevorrichtung"](#demoprojekt-biegevorrichtung)

## Über das Projekt

Mit dem Ziel einer Einführung von Vuforia Studio am Hans-Böckler-Berufskolleg Münster zur Unterstützung des Technikunterrichts zur Förderung der digitalen Schlüsselkompetenzen im Bereich der Aufbau- und Funktionsanalyse anspruchsvoller technischer Systeme. Wurde eine Schulung zu den Schlüsselkonzepten in Vuforia Studio gegeben, welche in diesem Repoitory festgehalten werden sollen.
Diese Dokumentation dient also zur Zusammenfassung des gelernten und bietet die Möglichkeit das Projekt Schritt für Schritt zu widerholen um die Techniken und Griffe zu verinnerlichen.
    Hierfür die Umsetzung eines Beispielprojektes "Biegevorrichtung"
<p align="right">(<a href="#top">back to top</a>)</p>

### Entwickelt mit

* [Vurofia Studio](https://www.ptc.com/de/products/vuforia/vuforia-studio)

<p align="right">(<a href="#top">back to top</a>)</p>

## Getting Started

### Voraussetzungen

* Eine lokale Installation von [Vuforia Studio](https://www.ptc.com/en/success-paths/develop-first-vuforia-studio-experience/setup/install-vuforia-studio-software)
* Ein - oder mehrere [Thingmarks](https://support.ptc.com/help/vuforia/studio/en/index.html#page/Studio_Help_Center/Widget3DMarker.html) für das Testen der App

### Vuforia Experience Server

Experience Kundenserver: https://vf.dev.cpronect.de

Log-in: Wurde zur Verfügung gestellt

### Installation

1. Vuforia Studio ausführen
   * Auf öffnen klicken
   * Bestenfalls Google Chrome nutzen
     
     ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/d2554545-d177-487e-b540-fd85e2b34fee)
2. Vuforia konfigurieren
   * Oben Rechts au die 3 Punkte klicken
   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/331a6b2e-38ad-4ed3-8206-7d53809f2c23)
    * Einstellungen auswählen
      
   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/d4031edc-6f29-45de-a68c-fab98f19d47f)
    * Die Service URL und log-in Daten eingeben
   
   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/a09ed508-104c-475b-bfde-8b9a2c6966cc)
    * Die Proxy Server URL kann leer bleiben
    * Debugprotokollierung und Schatten in 3D-Canvas zur Designzeit kann ebenfalls ignoriert werden

### Grundfunktionen

* Vuforia Studio bietet einen 3D - Canvas im Browser
* Eine Auflistung und Anleitung aller Funktionen von Vuforia Studio gibt es im PTC Helpcenter, siehe
    * [Vuforia Studio Basics](https://support.ptc.com/help/vuforia/studio/de/)

### Javascript

* Vuforia Studio bietet einen Editor im Browser an. 
* Alternativ kann auch eine eigene IDE / ein Text Editor genutzt werden.

> Vuforia Studio speichert selbstständig Javascript Code. Achte bei der Verwendung einer eigenen IDE unbedingt darauf, dass lokale Änderungen nicht überschrieben werden!

* Der Javascript Code befindet sich im Ordner `src/phone/components/Home.js`
* Weitere Module können mit zusätzlichen Views hinzugefügt werden.
* Für weitere Informationen, siehe
  * [Vuforia Studio Javascript Basics](https://support.ptc.com/help/vuforia/studio/en/index.html#page/Studio_Help_Center%2Fjs_basics.html%23)

<p align="right">(<a href="#top">back to top</a>)</p>

___
___

## Demoprojekt "Biegevorrichtung"
### Vorbereitung
* Alle notwendigen Dateien (Bilder, CAD-Daten, Videos etc.) befinden sich in diesem Repository unter `Ressourcen`
* Laden Sie am besten alle Ressourcen herunter, um die Demo direkt zu implementieren
### Erstellen einer neuen Experience 
1. Öffnen Sie Vuforia Studio.
2. Klicken Sie auf das grüne Plus in der oberen rechten Ecke, um ein neues Projekt zu erstellen.
   
   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/b6113ee7-fd74-49ad-930c-4ad3ed0da0e2)
4. Wählen Sie Mobilgerät - Standard als Vorlagentyp aus.
5. Geben Sie im Fenster Projektname `Biegevorrichtung Demo` ein, und geben Sie Ihre Experience Service URL an. Klicken Sie auf Erstellen.
6. Die Entwicklungsumgebung von Vuforia Studio wird nun geöffnet.

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/7f3840b8-58b3-4b8f-9035-9df88529290f)
### Einfügen eines 3D-Modells
1. Ziehen Sie ein Modell-Widget auf die mittlere Canvas, und legen Sie es ab. In der Canvas wird ein Standard-"Würfel" angezeigt, der das 3D-Modell darstellt.

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/0ae23ccf-490e-482c-8ebe-e9db1e7d77e4)
2. Klicken Sie bei ausgewähltem Modell unter EIGENSCHAFTEN auf das grüne + Zeichen neben dem Dropdown-Menü unter dem Feld Ressource.

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/4ab4e4b9-3ef2-47e8-a7c2-cd9d15ff1113)
3. Klicken Sie im Fenster Ressourcen hinzufügen (+) auf Dateien auswählen.
4. Navigieren Sie zu dem Speicherort, an den Sie die Ressourcen für diese Demo gespeichert haben, und wählen Sie die Datei [Biegevorrichtung_Hebel_Animationen.pvz](https://github.com/fstipp/Vuforia-Studio-HBBK/blob/main/ressources/Biegevorrichtung_Hebel_Animationen.pvz) aus. Klicken Sie auf Öffnen.
5. Klicken Sie im Fenster Ressourcen hinzufügen auf Hinzufügen.

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/fc90c003-1158-4f99-b14f-fe50310bd05a)
6. In der Canvas wird nun das 3D-Modell angezeigt

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/402d2d77-2620-4b64-b050-59e2d7d6919d)
> Das 3D-Modell `Biegevorrichtung_Hebel_Animationen.pvz` enthält bereits Animationen, die im vorhinein mithilfe von PTC Creo Illustrate erstellt wurden. Generell lassen sich aber alle gängigen 3D-Dateien auf die Canvas einfügen. Um später Einzelteile einer Baugruppe anprechen zu können empfiehlt sich das `.step` Format

7. Sobald Sie die Datei `Biegevorrichtung_Hebel_Animationen.pvz` hinzugefügt haben, wird die Dropdown-Liste Sequenz automatisch mit der Datei `Hebel Sequenz` gefüllt. Wählen Sie sie aus, um dem Modell die Hebel-Animationssequenz hinzuzufügen und die korrekte Darstellung des Modells herzustellen.

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/adc8a321-2db1-4bbc-88f5-a97fd66e87e3)
8. Klicken Sie in der Mitte oben in der Canvas auf das Symbol Transformieren.

    ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/5b72ae36-51a9-45f1-bfca-d7911190f998)
9. Klicken Sie auf den roten Bogen des Tools Transformieren, und ziehen Sie, bis das Modell um 90 Grad im Uhrzeigersinn gedreht ist. X-, Y- und Z-Koordinate werden durch die Farbe angezeigt, wobei Rot für X, Grün für Y und Blau für Z steht.
> Alternativ können Sie den Wert -90 im Feld X-Drehung für die Modelleigenschaften eingeben.






