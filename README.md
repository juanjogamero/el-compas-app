<div align="center">

<img src="app/src/main/res/drawable/logo.png" width="150" alt="El Compás" />

# El Compás

**Andalucía no se explica, se siente en cada compás.**

Una aplicación Android nativa para explorar cultura, personajes, música, vídeos y animaciones de Andalucía.

[Explorar presentación web](https://juanjogamero.github.io/el-compas-app/) · [Ver capturas](#capturas-de-pantalla) · [Código fuente](app/src/main)

![Android](https://img.shields.io/badge/Android-API%2024%2B-3DDC84?style=flat-square&logo=android&logoColor=white)
![Java](https://img.shields.io/badge/Java-11-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-KTS-02303A?style=flat-square&logo=gradle&logoColor=white)
![Media3](https://img.shields.io/badge/Media3-ExoPlayer-EC6D5C?style=flat-square)
![Lottie](https://img.shields.io/badge/Lottie-Animations-00B59C?style=flat-square)

</div>

---

## El proyecto

**El Compás** es una aplicación Android desarrollada en Java para explorar la cultura andaluza a través de una experiencia visual y multimedia. Reúne contenidos de personajes, vídeos, sonidos y animaciones en una interfaz personalizada.

La aplicación es **nativa para Android**. El sitio de GitHub Pages es una **presentación visual con capturas**, no una conversión ejecutable de la aplicación.

## Capturas de pantalla

<div align="center">

| Inicio | Personajes | Vídeos |
|:--:|:--:|:--:|
| <img src="screenshots/inicio.png" width="230" alt="Inicio"/> | <img src="screenshots/personajes.png" width="230" alt="Personajes"/> | <img src="screenshots/videos.png" width="230" alt="Vídeos"/> |

| Sonidos | Animaciones |
|:--:|:--:|
| <img src="screenshots/sonidos.png" width="230" alt="Sonidos"/> | <img src="screenshots/animaciones.png" width="230" alt="Animaciones"/> |

</div>

## Funcionalidades

| Módulo | Descripción |
| --- | --- |
| Inicio | Pantalla principal de presentación y acceso a las secciones |
| Personajes | Fichas con información de figuras y personajes populares |
| Vídeos | Reproducción mediante Media3 ExoPlayer |
| Sonidos | Reproductor musical con Android MediaPlayer |
| Animaciones | Animaciones JSON integradas con Lottie |

También se incluyen navegación inferior personalizada, listas con RecyclerView y adaptadores, controles multimedia y gestión del ciclo de vida de los reproductores.

## Stack técnico

- **Java 11** y Android SDK, con mínimo **API 24**.
- **Gradle Kotlin DSL** para compilación.
- **Material Components, AppCompat y ConstraintLayout** para la interfaz.
- **RecyclerView** para las listas de contenido.
- **Android MediaPlayer y Media3 ExoPlayer** para audio y vídeo.
- **Lottie** para animaciones.
- **GitHub Pages** para mostrar las capturas y las características de la aplicación.

## Estructura del repositorio

```text
app/src/main/
├── java/com/andalucia_app/
│   ├── MainActivity.java
│   ├── SplashActivity.java
│   ├── InicioFragment.java
│   ├── PersonajesFragment.java
│   ├── VideosFragment.java
│   ├── SonidosFragment.java
│   ├── AnimacionesFragment.java
│   ├── adapter/
│   └── entity/
└── res/
    ├── drawable/
    ├── layout/
    ├── raw/
    └── values/

docs/
└── index.html             # Presentación visual

screenshots/                # Capturas originales Android
.github/workflows/pages.yml # Despliegue de la presentación
```

## Ejecutar Android

Requisitos: Android Studio, Android SDK API 36, JDK compatible con el proyecto y un dispositivo o emulador Android 7.0 o superior.

```bash
git clone https://github.com/juanjogamero/el-compas-app.git
cd el-compas-app
./gradlew assembleDebug
```

También puedes abrir el proyecto con Android Studio y ejecutar la configuración `app`.

> La compilación Android no se ha verificado en esta actualización. Algunos recursos multimedia están incluidos en el proyecto; asegúrate de tener los derechos necesarios antes de redistribuirlos.

## Presentación en GitHub Pages

El workflow `.github/workflows/pages.yml` publica la carpeta `docs/`.

1. Abre **Settings → Pages** y selecciona **GitHub Actions** en *Source*.
2. Desde **Actions**, ejecuta **Deploy El Compas showcase to GitHub Pages** en la rama `main`.
3. Después del despliegue correcto, abre [El Compás](https://juanjogamero.github.io/el-compas-app/).

---

<div align="center">
  <strong>El Compás</strong><br/>
  <sub>Proyecto Android · Cultura andaluza</sub>
</div>
