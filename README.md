# 📱 Cómo Conectar tu Dispositivo Android
![image](https://github.com/user-attachments/assets/e1c34e6b-e92b-4b9c-bf43-644790bafe0d)
![image](https://github.com/user-attachments/assets/c62f3d8d-1cb6-468c-99d7-22c48a2819a9)

Este documento detalla los pasos para conectar tu dispositivo Android y ejecutar una aplicación en él.

## 📌 Índice

1. [Antes de comenzar](#antes-de-comenzar)
2. [Mira el video con instrucciones para compilar (opcional)](#mira-el-video-con-instrucciones-para-compilar-opcional)
3. [Cómo habilitar la depuración por USB](#como-habilitar-la-depuracion-por-usb)
4. [Cómo ejecutar tu app en el dispositivo Android con un cable](#como-ejecutar-tu-app-en-el-dispositivo-android-con-un-cable)
5. [Cómo ejecutar tu app en el dispositivo Android mediante Wi-Fi](#como-ejecutar-tu-app-en-el-dispositivo-android-mediante-wi-fi)
6. [Solución de problemas](#solucion-de-problemas)
7. [Conclusión](#conclusion)

---

## 1️⃣ Antes de comenzar
Antes de conectar tu dispositivo Android, asegúrate de cumplir con los requisitos previos:
- Tener **Android Studio** instalado.
- Contar con un cable USB funcional o conexión Wi-Fi.
- Activar las **Opciones de desarrollador** en el dispositivo.

## 2️⃣ Mira el video con instrucciones para compilar (opcional)
Si es tu primera vez configurando un dispositivo, puedes ver el video de instrucciones en el siguiente enlace: https://youtu.be/kp692Pih_ks(#).

## 3️⃣ Cómo habilitar la depuración por USB
Para activar la depuración por USB en tu dispositivo Android:
1. Ve a **Configuración > Acerca del teléfono**.
2. Toca varias veces sobre **Número de compilación** hasta activar el modo desarrollador.
3. Regresa a **Configuración** y accede a **Opciones para desarrolladores**.
4. Activa la opción **Depuración por USB**.

## 4️⃣ Cómo ejecutar tu app en el dispositivo Android con un cable
Para ejecutar la app mediante USB:
1. Conecta tu dispositivo a la computadora con un cable USB.
2. En la ventana emergente del dispositivo, selecciona **Permitir depuración USB**.
3. Abre **Android Studio** y selecciona tu dispositivo en la barra de ejecución.
4. Haz clic en ▶️ para ejecutar la app.

## 5️⃣ Cómo ejecutar tu app en el dispositivo Android mediante Wi-Fi
Si prefieres conectar tu dispositivo sin cables:
1. Conéctalo mediante USB y ejecuta:
   ```sh
   adb tcpip 5555
   ```
2. Desconecta el cable y conecta tu dispositivo a la misma red Wi-Fi.
3. Obtén la IP del dispositivo en **Opciones para desarrolladores > Estado de red**.
4. En la terminal de tu PC, ejecuta:
   ```sh
   adb connect [IP_DEL_DISPOSITIVO]:5555
   ```
5. Selecciona el dispositivo en **Android Studio** y ejecuta la app.

## 6️⃣ Solución de problemas
Si encuentras problemas al conectar tu dispositivo:
- **Android Studio no reconoce el dispositivo:** Desconéctalo y vuelve a conectarlo o reinicia Android Studio.
- **Error de autorización:** Ve a **Opciones para desarrolladores > Revocar autorizaciones de depuración** y vuelve a conectar el dispositivo.
- **El emulador no funciona en Windows:** Verifica los **controladores USB de OEM**.

## 7️⃣ Conclusión
Siguiendo estos pasos, habrás conectado tu dispositivo Android y ejecutado tu aplicación correctamente. 🚀

## 📸 Capturas de pantalla
![Interfaz de conexión](image.png)

---
📢 ¡Si este documento te fue útil, no olvides dejar un ⭐ en el repositorio!
