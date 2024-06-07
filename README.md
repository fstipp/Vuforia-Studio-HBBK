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
- [Roadmap](#roadmap)

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
* Ein - oder mehrere [Thingmarks](https://support.ptc.com/help/vuforia/studio/en/index.html#page/Studio_Help_Center/Widget3DMarker.html) für das Testen mit der Hololens

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
### Einleitung
* Alle notwendigen Dateien (Bilder, CAD-Daten, Videos etc.) befinden sich in diesem Repository unter `Ressourcen`  
### Erstellen einer neuen Experience 
