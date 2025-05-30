# 4. Creació d'un projecte

## 4.1. Configuració

- Per a crear un nou projecte farem com sempre: `File` → `New Project`
- A continuació, configurarem el tipus de projecte.
  - Seleccionarem la Categoria *Java with Ant* i dins d’aquesta JavaFX.
  - En **Projects** triarem *JavaFX FXML Application* i polsarem `Next`.
  - Anomenem el projecte i seleccionem la plataforma que hem creat.

![Imatge 3](/uf11/nou_projecte.jpg)

![Imatge 3](/uf11/nou_projecte_nom.jpg)

- Una vegada tenim el projecte creat hem d’afegir la llibreria que hem creat de JavaFX.
  - Ens situarem en la carpeta Libraries i polsarem botó dret.
  - Seleccionarem l’opció `Add Library`.
  - Cercarem la llibreria JavaFX i polsarem `Add Library`. Veurem com s’ha incorporat el conjunt de llibreries.

Podem fer una prova executant la classe principal.

![Imatge 3](/uf11/add_library.jpg)

![Imatge 3](/uf11/add_javaFX.jpg)

![Imatge 3](/uf11/run_file.jpg)

![Imatge 3](/uf11/run.jpg)

## 4.2. Estructura

El nostre projecte està dividit en tres parts.

- **VISTA (FXMLDocument.fxml)**:
Es tracta d’un arxiu en format fxml. Si polsem botó dret i Editar verem el contingut. Si fem doble clic s’obrirà la visualització en Scene Builder on podrem dibuixar la part gràfica
amb contenidors i objectes gràfics.

- **CONTROLADOR (FXMLDocumentController.java)**:
Al controlador, utilitzant les classes de JavaFX, programarem els mecanismes mitjançant els quals interactuarem tant amb la vista com amb el programa. Aquesta classe l'haurem d'identificar a Scene Builder. Crearem els mètodes que gestionen els esdeveniments.

- **PROGRAMA (programa.java)**:
On desenvoluparem la nostra lògica.
Utilitzarem els mètodes GET i SET dels objectes gràfics.
