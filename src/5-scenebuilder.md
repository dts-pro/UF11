# 5. Scene Builder

## 5.1. Entorn

Si obrim l'arxiu *FXMLDocument.fxml* (doble clic) se'ns obrirà Scene Builder on podrem, d'una manera gràfica, fer canvis sobre la interfície.

![Esquema d'herència](/uf11/Scene_builder_editor.jpg)

## 5.2. Secció Library

<div style="display: flex; gap: 50px">

<div style="flex: 1; padding: 10px; text-align: justify;">

  En el panell dret de Scene Builder es pot trobar aquesta secció que engloba diversos apartats com: 
  Contenidors, Controls, Menú, etc. És a dir, els elements gràfics que es poden afegir a la interfície gràfica.

  Dins de tots aquests apartats cal destacar <strong>Contenidors (Layouts)</strong>, on es troben els diferents tipus de 
  contenidors que permeten organitzar els elements que es vulguen afegir al disseny, i <strong>Controls</strong>, que conté 
  els elements més comuns de la majoria de les interfícies gràfiques.

</div>

  ![Esquema d'herència](/uf11/panel_elements.jpg)

</div>

<div style="display: flex; gap: 50px">

<div style="flex: 0.8; padding: 10px; text-align: justify;">

  **Per a afegir un element al disseny, tan sols has d'arrossegar-lo** cap al lloc desitjat, tenint en compte que els elements com els controls sempre han de col·locar-se dins d'un element de tipus contenidor.

  Per defecte es crea un contenidor general de tipus **AnchorPane**, que són els que permeten col·locar elements de manera bastant lliure, ancorant els elements respecte a la posició d'uns altres.

</div>

<div style="flex: 0.8; padding:10px;">

<div style="margin-top: 90px;"> <!-- Aquest div fa que tot quede més baix -->
</div>

  ![Esquema d'herència](/uf11/Scene_builder_editor_afegir_element.jpg)

</div>
</div>

## 5.3. Secció Documents

<div style="display: flex; gap: 50px">

<div style="flex: 0.9; padding: 10px; text-align: justify;">

  Aquesta secció només inclou els apartats **Hierarchy** (jerarquia) i **Controller**.

  En l'apartat **Hierarchy** pots veure de manera detallada quins elements estan continguts dins d'uns altres, i pot resultar de bastant utilitat quan desitges reorganitzar els elements dins dels diferents contenidors que tingues en el disseny.

  En aquest exemple dins del contenidor principal (AnchorPane) s'ha col·locat un contenidor vertical (VBox) dins del qual hi ha 2 contenidors horitzontals (HBox) amb alguns controls.

</div>

<div style="flex: 0.8; padding:10px;">

<div style="margin-top: 90px;"> <!-- Aquest div fa que tot quede més baix -->
</div>

![Esquema d'herència](/uf11/hierarchy.jpg)

</div>
</div>

<div style="display: flex; gap: 50px">

<div style="flex: 1; padding: 10px; text-align: justify;">

  En l'apartat Controller pots veure i modificar el nom de la classe que farà les funcions de controladora d'aquest arxiu FXML.

  També mostra els identificadors que s'han assignat als elements del disseny que el tinguen.

  S’ha de tindre en compte que si canvies el nom de la classe controladora des de NetBeans o la mous a un altre paquet de fonts, hauràs de canviar les noves dades en aquest apartat.

</div>

<div style="flex: 0.6; padding:10px;">

<div style="margin-top: 0px;"> <!-- Aquest div fa que tot quede més baix -->
</div>

![Esquema d'herència](/uf11/Controller.jpg)

</div>
</div>

---

## 5.4. Zona de Disseny

<div style="display: flex; gap: 50px">

<div style="flex: 1; padding: 10px; text-align: justify;">

  En la part central es troba la zona de disseny on es poden anar col·locant els diferents elements de la llibreria.
  
  Si es selecciona un determinat element es pot modificar la seua grandària estirant amb el ratolí des dels indicadors blaus de les cantonades o laterals.

  Obrint el menú contextual podràs trobar diverses accions que podràs realitzar sobre aqueix element.
  
</div>

<div style="flex: 0.7; padding:10px;">

<div style="margin-top: 0px;"> <!-- Aquest div fa que tot quede més baix -->
</div>

![Esquema d'herència](/uf11/zona_disseny.jpg)


</div>
</div>

---

## 5.5. Zona inspector

<div style="display: flex; gap: 50px">

<div style="flex: 1; padding: 10px; text-align: justify;">

El inspector conté els apartats **Properties**, **Layout**, i **Code**.

En l'apartat **Properties** podràs consultar i modificar els valors assignats a les propietats que ofereix l'element que es trobe seleccionat. Segons el tipus d'element que siga, es mostraran diferents propietats.

Ací es podrà canviar, per exemple, el text d'un element, el seu color, tipus de font, alineacions, o assignar-li un estil CSS a JavaFX.
  
</div>

<div style="flex: 0.7; padding:10px;">

<div style="margin-top: 0px;"> <!-- Aquest div fa que tot quede més baix -->
</div>

![Esquema d'herència](/uf11/inspectorproperties.jpg)

</div>
</div>

<div style="display: flex; gap: 50px">

<div style="flex: 1; padding: 10px; text-align: justify;">

L'apartat Layout permet consultar i modificar els aspectes relacionats amb la distribució de l'element en pantalla. És a dir, ací podràs assignar marges, grandàries, escales, etc.

En l'apartat Anchor Pane Constraints és podran definir els marges respecte al pare on es troba l'element.

</div>

<div style="flex: 0.8; padding:10px;">

<div style="margin-top: 0px;"> <!-- Aquest div fa que tot quede més baix -->
</div>

![Esquema d'herència](/uf11/isnpector_layout.jpg)

</div>
</div>

<div style="display: flex; gap: 50px">

<div style="flex: 0.9; padding: 10px; text-align: justify;">

L'apartat **Code** permet configurar una part del codi. Es poden codificar els events de teclat, ratolí, touch (per a pantalles tàctils), etc. que després es gestionaran des de l’arxiu Controller.

</div>

<div style="flex: 0.7; padding:10px;">

<div style="margin-top: 0px;"> <!-- Aquest div fa que tot quede més baix -->
</div>

![Esquema d'herència](/uf11/inspector_code.jpg)

</div>
</div>

## 5.6. Make Controller

<div style="display: flex; gap: 50px">

<div style="flex: 0.9; padding: 10px; text-align: justify;">

Després de qualsevol canvi que es realitze en l'apartat Code, i després de guardar els canvis de l'arxiu en Scene Builder, s’ha d'actualitzar la informació en la classe controladora de NetBeans.

Per a fer-ho s’hi ha d'utilitzar l'opció **`Make Controller`** del menú contextual de l'arxiu FXML en NetBeans.

És a dir, si s'indica un nom d'un mètode per a una acció, per exemple, quan l'usuari moga el ratolí dins del botó, s'ha de seleccionar Make Controller perquè es declare aquest mètode en el controlador.

</div>

<div style="flex: 0.7; padding:10px;">

<div style="margin-top: 60px;"> <!-- Aquest div fa que tot quede més baix -->
</div>

![Esquema d'herència](/uf11/make_controller.jpg)

<div style="margin-top: 20px;"> <!-- Aquest div fa que tot quede més baix -->
</div>

![Esquema d'herència](/uf11/make_controller2.jpg)

</div>
</div>

Cal recordar prémer la tecla Intro després d'escriure el nom de l'identificador o d'un mètode perquè es tinga en compte aquest nom en guardar el document FXML des de Scene Builder.

![Esquema d'herència](/uf11/make_controller_codi.jpg)


---
