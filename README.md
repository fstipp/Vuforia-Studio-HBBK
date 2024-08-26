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

Mit dem Ziel einer Einführung von Vuforia Studio am Hans-Böckler-Berufskolleg Münster zur Unterstützung des Technikunterrichts zur Förderung der digitalen Schlüsselkompetenzen im Bereich der Aufbau- und Funktionsanalyse anspruchsvoller technischer Systeme. Wurde eine Schulung zu den Schlüsselkonzepten in Vuforia Studio gegeben, welche in diesem Repository festgehalten werden sollen.
Diese Dokumentation dient also zur Zusammenfassung des gelernten und bietet die Möglichkeit das Projekt Schritt für Schritt zu wiederholen, um die Techniken und Griffe zu verinnerlichen.
    Hierfür die Umsetzung eines Beispielprojektes "Biegevorrichtung"
<p align="right">(<a href="#top">back to top</a>)</p>

### Entwickelt mit

* [Vuforia Studio](https://www.ptc.com/de/products/vuforia/vuforia-studio)

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
   * Oben rechts auf die 3 Punkte klicken
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

7. Sobald Sie die Datei `Biegevorrichtung_Hebel_Animationen.pvz` hinzugefügt haben, wird die Dropdown-Liste Sequenz automatisch mit der Datei `Hebel Sequenz` gefüllt. Wählen Sie sie aus, um dem Modell die Hebel-Animationssequenz hinzuzufügen.

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/83bf6e7e-a5d7-4b54-a424-9dae6e0f9e4e)
8. Klicken Sie in der Mitte oben in der Canvas auf das Symbol Transformieren.

    ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/5b72ae36-51a9-45f1-bfca-d7911190f998)
9. Klicken Sie auf den roten Bogen des Tools Transformieren, und ziehen Sie, bis das Modell um 90 Grad im Uhrzeigersinn gedreht ist. X-, Y- und Z-Koordinate werden durch die Farbe angezeigt, wobei Rot für X, Grün für Y und Blau für Z steht.
> Alternativ können Sie den Wert -90 im Feld X-Drehung für die Modelleigenschaften eingeben.
10. Klicken Sie bei weiterhin ausgewähltem Werkzeug Transformieren auf die Pfeile, und ziehen Sie, bis das Modell da platziert ist, wo Sie es platzieren möchten.
11. Klicken Sie auf Speichern.

### Einfügen eines ThinkMarks
Experiences in Vuforia View werden durch das Scannen des ThingMarks von Ihrem Gerät angezeigt. Damit das 3D-Modell an der richtigen Stelle angezeigt wird, müssen Sie ein digitales ThingMark an derselben Stelle platzieren wie Ihr reales ThingMark. Wenn Sie beispielsweise möchten, dass das gedruckte ThingMark als Tischoberfläche für Ihre AR-Szene dient, platzieren Sie das ThingMark im Vuforia Studio unter dem Modell. Wenn Sie möchten, dass das gedruckte ThingMark auf die Oberfläche eines physischen Objekts angewendet wird, platzieren Sie das ThingMark entsprechend im Vuforia Studio.

1. Ziehen Sie ein ThingMark Widget in die Canvas, und legen Sie es ab.

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/c2c30cc6-bd01-4494-aa8d-5a50aeb83b57)
   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/84b9afbe-cef3-45e5-8a3a-f1b76e81260f)

Die Platzierung des ThingMark in Vuforia Studio entspricht direkt der Position, an der das AR-Erlebnis das Modell in Vuforia View platziert.
Das gilt auch für die Drehung. Sie sollten entweder das digitale ThingMark genauso drehen, wie es in der Wirklichkeit platziert wird, oder die ThingMark in der Wirklichkeit so drehen, dass ihre Ausrichtung der in Vuforia Studio entspricht.
> Für das Demoprojekt kann auch das räumliche Ziel (spartial Target) benutzt werden - Das vorgehen ist identisch

### 3D-Bild einfügen
1. Ziehen Sie ein 3D-Bild Widget in die Canvas
2. Wählen Sie die Ressource des Bildes aus `explosionsdarstellung.png`

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/0c2457dd-157f-4fe1-b8dd-051f47412a8c)
3. Nutzen Sie das `Skalierung`-Feld und die bunten Transformationspfeile, um das Bild korrekt auszurichten

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/73791367-ef7c-4e3d-b07c-c226df23b130)

### Animation abspielen
Sofern auf dem 3D-Modell bereits Animationen hinterlegt sind, lassen sich diese ganz einfach abspielen. In diesem Beispiel wollen wir die hinterlegte Animation per Tippen auf das Modell auslösen - Möglich sind aber auch Buttons oder Bilder als Auslöser hierfür.
1. Im Strukturbaum das Modell auswählen (model-1) und bei den Eigenschaften nach ganz unten scrollen

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/e8332138-5944-4415-8d37-16adcdc00495)
2. Das `Klicken` Event an dem Pfeil ziehen und per Drag and Drop auf das 3D-Modell legen

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/99d5b8f3-bfd4-4429-8e74-4010ec040d68)
3. Es öffnet sich nun ein Pop-Up Fenster - Wählen Sie hier `Alle widergeben` als Bindungsziel aus und klicken sie auf `Binden`

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/0a6c6f2b-b95b-449b-9cb5-ef1edbda4aea)

> Tipp: Sie können ihre Experience immer mal wieder Testen in dem Sie oben auf `Preview` bzw. `Vorschau` klicken. Es öffnet sich dann eine Simulation der App im Browser, in dieser können Sie schauen ob, die von Ihnen implementierten Funktionen korrekt sind.

### 2D-Buttons einfügen
Da jetzt der 3D-Anteil Ihres Erlebnisses fertig ist, lassen Sie uns einige 2D-Elemente hinzufügen.
1. Klicken Sie in der Canvas-Symbolleiste auf 2D.
  
   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/7ff2e014-0970-42e5-a0ba-b447e9e5de72)
2. Navigieren Sie im Fensterbereich PROJEKT zu `Ansichten > Startseite > 2D-Überlagerung`.
3. Ziehen Sie ein Raster-Layout-Widget auf den unteren Bereich, und legen Sie es ab.

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/141314b4-efa1-4ed2-bc00-85bf2dc7fd1f)
4. Ziehen Sie ein Umschalten-Widget in das Raster-Layout

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/d92cb6d0-fdfd-4bba-a25c-f8ec05fa5d5e)

5. Navigieren Sie im Fensterbereich PROJEKT zu `Ansichten > Startseite > 2D-Überlagerung > 2D-Körper > Unterer Bereich > gridLayout-1 > row-1` und klicken Sie auf den Eintrag `column-1`, um ihn auszuwählen.
6. Setzen Sie die beiden Ausrichtungen auf Mitte

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/7ae26d3a-a110-426e-8fc4-6e347f4e200d)
7. Navigieren Sie wieder zu dem Umschalten-Widget und ändern Sie in den Eigenschaften die Beschriftung zu `Explosionsdarstellung`

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/797a4bed-ae91-4826-9195-9a0c0fa8e070)

> Ziel ist es nun den Toogle-Button bzw. die Umschaltung so zu verbinden, dass auf Knopfdruck das 3D-Bild verschwindet und beim 'entdrücken' dieses wieder erscheint.

8. Ziehe dazu in den Eigenschaften des Umschalt-Widgets das Bindingsymbol neben der Eigenschaft `Wert` ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/d4eba904-5a92-4446-b116-2f1404c156a0) auf das 3D-Image im Strukturbaum.

   ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/14c07ef0-f97f-4722-b61c-18a78d5e59d2)
9. Wähle die Eigenschaft `Sichtbar` als Bindungsziel und klicken Sie auf Binden.

    ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/fc75829d-03fc-4cc9-8393-5d6875a9d40e)

### Animationen in Vuforia Studio erstellen
Falls Creo Illustrate für das erstellen von Animationen nicht zur Verfügung steht, gibt es auch die Möglichkeit mithilfe des Einsatzes von JavaScript-Codes Teile des Modells zu bewegen. Dazu müssen wir zunächst im Modell alle Teile "markieren", welche wir animieren wollen. 
Ziel ist es eine Explosionsdarstellung zu erstellen.

1. Navigieren Sie zunächst wieder auf die 3D-Ansicht der Experience ![image](https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/ea030e4c-2d64-4fbf-ab1f-984ffbbc7c49)

2. Ziehen Sie nun ein Modellelement-Widget auf den Teil des 3D-Modells, welchen Sie bewegen möchten.

   <img width="708" alt="image" src="https://github.com/fstipp/Vuforia-Studio-HBBK/assets/119317738/2da27f9f-863d-4fd3-89fa-6df36f754a5e">
> Achtung: Hierfür muss dieser Teil des Modells eine eigene Komponente in dem zugrunde liegenden CAD-Modell sein.
3. Das Teil wird in der Canvas farblich hervorgehoben und ist nun auch einzeln ansteuerbar unter dem namen `modelItem-2`

  ![image](https://github.com/user-attachments/assets/6b88ca6c-a55e-4855-bbd9-85266eaed31d)

4. Dieser Schritt wird jetzt wiederholt angewendet für jedes Teil, welches Sie in der Explosionsanimation bewegen möchten. Für die Biegevorichtung ergib dies insgesamt 15 einzelteile, die wir definieren müssen.

   ![image](https://github.com/user-attachments/assets/19c4ff35-7cbe-4592-ba81-1d5875d0c9b4)

5. Um die Einzelnen Teile nun über JavaScript bewegen zu können navigieren Sie als nächstes in der linken leiste zu `Home.js` bzw. `Startseite.js`

     ![image](https://github.com/user-attachments/assets/7ad0b9f5-1f95-4a6f-bad8-3f4deb3dc4d0)

6. Fügen Sie den folgenden Code ein
```javascript
   var explosionsansicht  = false;

$scope.press_explosion = function () {
    function startExplosion(direction) {
    var counter = 0
    function animate() {
      if (counter < 360) {
        	counter += 1
        // Hier werden alle Teile aufgeführt, welche bewegt werden sollen
        
        // Buchse + Hebel
       	$scope.view.wdg['modelItem-1'].z += direction * 0.0003;
        $scope.view.wdg['modelItem-2'].z += direction * 0.0003;
        $scope.view.wdg['modelItem-3'].z += direction * 0.0003;
        
        // Bolzen
        $scope.view.wdg['modelItem-4'].z += direction * 0.00055;
        
        // usw.
        $scope.view.wdg['modelItem-5'].z += direction * 0.0002;
        $scope.view.wdg['modelItem-6'].z += direction * 0.00025;
        $scope.view.wdg['modelItem-7'].z += direction * 0.0002;
        
        $scope.view.wdg['modelItem-8'].z += direction * 0.00019;
        $scope.view.wdg['modelItem-9'].z += direction * 0.00025;
        
        $scope.view.wdg['modelItem-10'].z += direction * 0.0002;
        
        $scope.view.wdg['modelItem-11'].z += direction * 0.00015;
        
        $scope.view.wdg['modelItem-12'].z += direction * 0.0001;
        $scope.view.wdg['modelItem-13'].z += direction * 0.0001;
        
        $scope.view.wdg['modelItem-14'].z += direction * 0.00003;
        
        
        ////
        	$timeout(animate, 5);
      } 
    }
    animate();
    }
      
    explosionsansicht = !explosionsansicht;
    startExplosion(explosionsansicht ? 1 : -1)
  };
   ```
Nachdem der Code implementiert ist, gibt es einige zusätzliche Anpassungsmöglichkeiten:

-  **Richtungsachse anpassen**: Anstelle der `z`-Achse können auch die `x`- oder `y`-Achsen verwendet werden, um die Teile in andere Richtungen zu bewegen. Ersetzen Sie dafür einfach `.z` durch `.x` oder `.y` im Code.

-  **Bewegungsweite steuern**: Die Zahl, die mit dem `direction`-Parameter multipliziert wird (z.B. `0.0003`), bestimmt, wie weit die Teile sich bewegen. Ein höherer Wert lässt die Teile weiter fliegen, während ein niedrigerer Wert die Bewegung entsprechend reduziert.

Diese Flexibilität ermöglicht es Ihnen, die Animation an Ihre spezifischen Bedürfnisse anzupassen und verschiedene visuelle Effekte zu erzielen.

> Beachten Sie, dass die Wirkung der Animation stark von der Zuordnung der ModelItems im Projekt abhängt. Es ist empfehlenswert, das Demoprojekt als Referenz zu verwenden, um die Animation genau nachzubilden. Auch ohne diese Referenz kann die Animation funktionieren, allerdings müssen möglicherweise die Parameter der ModelItems angepasst werden, um die gewünschten Effekte zu erreichen.

7. Um die gerade implementierte Animation abzuspielen verwenden wir den 2D-Button den wir zuvor erstellt haben. Navigieren Sie dazu im Struktubaum zu `toggle-1` 

   ![image](https://github.com/user-attachments/assets/9d0440f8-124c-41a0-a14e-8bf413958157)

8. Klicken Sie unten in den Eigenschaften auf `JS`-Symbol neben "Klicken"

 ![image](https://github.com/user-attachments/assets/82031b8d-222d-405b-a1b2-eb61e472e9bd)

9. Es öffnet sich ein kleines Textfeld - geben Hier hier `press_explosion();` ein

    ![image](https://github.com/user-attachments/assets/5f7edf33-57b2-4ed5-8ddb-3b6ea7051676)

10. Nun speilt die Anmation, immer wenn Sie den Button "Explosionsdarstellung" drücken.

    ![image](https://github.com/user-attachments/assets/efceec9a-a09f-4f60-99d2-b1c613db98e3)
 







