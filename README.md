# YouTube a MP3 (con yt-dlp y ffmpeg)

Este programa permite descargar el **audio en MP3** de un video de YouTube con la mejor calidad disponible (**320 kbps**).  
Está desarrollado en **Python**, con una interfaz gráfica hecha en **Tkinter**, y empaquetado en **.exe** para que funcione en cualquier PC con Windows.

---

## 📌 Requisitos

Para ejecutar el script en Python necesitas:

- **Python 3.8 o superior**  
- **pip** (gestor de paquetes de Python)  
- **yt-dlp** (se instala con `pip install yt-dlp`)  
- **Tkinter** (incluido por defecto en Python para Windows)  
- **ffmpeg.exe, ffplay.exe y ffprobe.exe** en la misma carpeta que el script, o instalados en el PATH de Windows  

⚠️ Si usas la versión compilada (`youtube.exe`), ya no necesitas instalar nada:  
el programa incluye `ffmpeg.exe` junto al ejecutable.

---

## 📂 Estructura de carpetas (para la versión .exe)

Cuando generes el ejecutable con PyInstaller, distribuye el proyecto así:

YouTubeMP3/
│
├─ youtube.exe # Ejecutable principal
├─ ffmpeg.exe # Necesario para la conversión
└─ _internal/ # Carpeta generada automáticamente por PyInstaller


El usuario solo debe descomprimir y ejecutar `youtube.exe`.

---

## 🚀 Uso

### Opción 1: Ejecutar como script de Python
1. Clona este repositorio o descarga los archivos.
2. Instala dependencias:
   ```bash
   pip install -r requirements.txt

3. Asegúrate de tener ffmpeg.exe en la misma carpeta que youtube.py.

4. Ejecuta el programa:
python youtube.py

Opción 2: Ejecutar como programa (.exe)

Descarga el ZIP con youtube.exe y ffmpeg.exe.

Descomprime en una carpeta.

Haz doble clic en youtube.exe.

Pega la URL de un video de YouTube y se descargará en tu carpeta Descargas como MP3.