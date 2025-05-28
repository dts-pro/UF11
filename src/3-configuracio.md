# 3. Configuració

## 3.1. Verificacions i instal·lacions

- Per a comprovar la versió de **NetBeans** instal·lada, anirem al menú **`Help` → `About`**. Si no tenim una versió recent (actualment la 25), caldria reinstal·lar-la.

- Per a instal·lar **Scene Builder**:
  1. Accedir a la [web oficial](https://gluonhq.com/products/scene-builder/).
  2. Descarregar l'instal·lador corresponent al sistema operatiu.
  3. Executar l'instal·lador per a completar la instal·lació.

- Per a instal·lar **JavaFX**
  1. Anar a la [web](https://gluonhq.com/products/javafx/).
  2. Descarregar l'arxiu `.zip` de JavaFX.
  3. Descomprimir l'arxiu en la carpeta on tenim Java.

- Per a instal·lar **Java JDK FX**
  1. Anar a la [web](https://www.azul.com/downloads/?package=jdk-fx#zulu).
  2. Buscar l'última versió **(Java 23)**, i descarrega el **Java Package JDK FX** adequat per al teu sistema operatiu i arquitectura.
  3. Descomprimix-lo en la carpeta on tenim Java.
     • Windows: `C:\Arxius de programa\Java\`
     • Linux: `usr/lib/jvm`
  4. Opcionalment, canviar-li el nom a `jdk-23-javafx` per a facilitar la identificació.

---

## 3.2. Instal·lar el plugin JavaFX

Anirem a activar i configurar el plugin de JavaFX.

- Ens dirigim a `Tools` → `Options` → `Java` → `JavaFX`.
- Seguirem els passos que ens va indicant.

<div style="border: 6px solid rgb(240, 102, 61); max-width: 100%; margin: 0 auto; text-align: center;">
    <img src="/uf11/tools_javafx.jpg" style="max-width: 100%; height: auto;" alt="Esquema d'herència">
</div>

---

## 3.3. Connectar Scene Builder

Quan polsem [Finish] el sistema ens mostrarà un avis indicant-nos que ha detectat i connectat Scene Builder.

D’aquesta manera NetBeans detectarà on està l’executable i farà ús d’aquest en el moment de la edició.

<div style="border: 6px solid rgb(240, 102, 61); max-width: 100%; margin: 0 auto; text-align: center;">
    <img src="/uf11/tools_javafx2.jpg" style="max-width: 100%; height: auto;" alt="Esquema d'herència">
</div>

---

## 3.4. Incloure la llibreria de JavaFX

El primer que haurem de fer és incloure la llibreria de JavaFX en les llibreries que utilitza NetBeans.

- Ens dirigim a `Tools` → `Libraries` → `New Library`
- Li donem nom Library Name: "JavaFX", acceptem i polsem `Add JAR/Folder`

<div style="display: flex; justify-content: center; gap: 20px;">

  <div style="border: 6px solid rgb(240, 102, 61); max-width: 100%; text-align: center;">
    <img src="/uf11/Tools_Libraries.jpg" style="max-width: 100%; height: auto;" alt="Imatge 1">
  </div>

</div>
 
<div style="display: flex; justify-content: center; gap: 20px;">

  <div style="border: 6px solid rgb(240, 102, 61); max-width: 100%; text-align: center;">
    <img src="/uf11/nom_javaFX.jpg" style="max-width: 100%; height: auto;" alt="Imatge 2">
  </div>

</div>

---

- Busquem la carpeta de JavaFX que hem descomprimit
- Accedirem a la subcarpeta *lib*
- Seleccionem els arxius (són tots .jar) i polsem `Add JAR/Folder`.
- Polsem `OK`

<div style="display: flex; justify-content: center; gap: 20px;">

  <div style="border: 6px solid rgb(240, 102, 61); max-width: 100%; text-align: center;">
    <img src="/uf11/ruta_lib.jpg" style="max-width: 100%; height: auto;" alt="Imatge 1">
  </div>

</div>
 
<div style="display: flex; justify-content: center; gap: 20px;">

  <div style="border: 6px solid rgb(240, 102, 61); max-width: 100%; text-align: center;">
    <img src="/uf11/llibreries_importades.jpg" style="max-width: 100%; height: auto;" alt="Imatge 2">
  </div>

</div>

---

## 3.5. Crear la plataforma

 Per raons de simplicitat, anem a optar per la categoria de projectes ***Java with Ant***. Açò ens portarà a haver de configurar una Plataforma per a desenvolupar projectes de JavaFX.

- Ens dirigirem a `Tools` → `Java Platform`
- Polsarem `AddPlatform`. En la següent pantalla no modificarem cap opció.
- Finalment triarem la carpeta que hem descarregat *jdk-23.02-javafx*.

<div style="display: flex; justify-content: center; gap: 20px;">

  <div style="border: 6px solid rgb(240, 102, 61); max-width: 100%; text-align: center;">
    <img src="/uf11/java_platform_manager.jpg" style="max-width: 100%; height: auto;" alt="Imatge 1">
  </div>

</div>
 
<div style="display: flex; justify-content: center; gap: 20px;">

  <div style="border: 6px solid rgb(240, 102, 61); max-height: 100%; text-align: center;">
    <img src="/uf11/add_platform.jpg" style="width: auto; height: 100%;" alt="Imatge 2">
  </div>

</div>
 
<div style="display: flex; justify-content: center; gap: 20px;">

  <div style="border: 6px solid rgb(240, 102, 61); max-width: 100%; text-align: center;">
    <img src="/uf11/seleccionar_javafx_platform.jpg" style="max-width: 100%; height: auto;" alt="Imatge 3">
  </div>

</div>

- Seleccionarem un nom significatiu per a la plataforma i finalitzarem la creació.

<div style="display: flex; justify-content: center; gap: 20px;">

  <div style="border: 6px solid rgb(240, 102, 61); max-width: 100%; text-align: center;">
    <img src="/uf11/nom_javafx_platform.jpg" style="max-width: 100%; height: auto;" alt="Imatge 3">
  </div>

</div>

---
