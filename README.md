# Publicación de Aplicaciones en Windows con .NET MAUI

## Descripción
Este proyecto consiste en la creación y despliegue de una aplicación de escritorio para Windows utilizando .NET MAUI. La aplicación mostrará el nombre y apellidos del desarrollador en la interfaz y se documenta el proceso de publicación e instalación con firma digital.

## Características
- Aplicación desarrollada con .NET MAUI.
- Implementación de una interfaz simple mostrando nombre y apellidos.
- Generación de un paquete de instalación (.MSIX).
- Firma digital del instalador.
- Instalación del certificado de confianza en el sistema.
- Publicación e instalación paso a paso con PowerShell.

## Tecnologías Utilizadas
- .NET MAUI
- C#
- Visual Studio
- PowerShell
- Certificados digitales

2. **Abrir en Visual Studio**
   - Abrir el archivo de solución `.sln` en Visual Studio.
3. **Configurar la Publicación**
   - En Visual Studio, ir a `Propiedades` del proyecto.
   - Configurar la publicación como `Paquete MSIX`.
4. **Generar el Instalador**
   - Clic en `Publicar` y seguir las instrucciones.
5. **Instalar el Certificado de Confianza**
   ```powershell
   Import-Certificate -FilePath "ruta_del_certificado.cer" -CertStoreLocation Cert:\LocalMachine\TrustedPeople
   ```
6. **Ejecutar el Instalador**
   - Abrir el archivo `.MSIX` generado y completar la instalación.

## Capturas de Pantalla
- 📌 Generación del paquete de instalación.
- 📌 Instalación del certificado en `certmgr.msc`.
- 📌 Ejecución de la aplicación instalada.

## Requisitos
- Windows 10/11.
- Visual Studio con .NET MAUI instalado.
- Permisos de administrador para instalar el certificado.

## Contribución
Si deseas contribuir, por favor sigue estos pasos:
1. Haz un **fork** del repositorio.
2. Crea una **rama** con tu nueva característica (`git checkout -b feature/nueva-feature`).
3. **Commitea** tus cambios (`git commit -m 'Añadir nueva característica'`).
4. Haz un **push** a la rama (`git push origin feature/nueva-feature`).
5. Abre un **Pull Request**.

## Autor
👤 **Piero Zavala Chira**

## Licencia
Este proyecto está bajo la licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.
