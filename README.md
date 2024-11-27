# MacManager

Gestor de Direcciones MAC - PowerShell
Este script en PowerShell permite gestionar fácilmente las direcciones MAC de los adaptadores de red en un equipo con Windows. Ofrece una interfaz interactiva con varias opciones, desde generar direcciones aleatorias hasta restaurar la dirección MAC predeterminada.

Características
Mostrar Interfaces de Red Disponibles

Lista las interfaces de red activas con detalles como estado, dirección MAC actual y velocidad de enlace.
Ver Dirección MAC Actual de una Interfaz

Muestra la dirección MAC configurada actualmente para una interfaz específica.
Cambiar Dirección MAC a una Aleatoria

Genera automáticamente una nueva dirección MAC válida y la aplica a la interfaz seleccionada.
Cambiar Dirección MAC Manualmente

Permite al usuario ingresar una dirección MAC personalizada en el formato XX-XX-XX-XX-XX-XX.
Restaurar Dirección MAC Predeterminada

Elimina cualquier dirección MAC personalizada y restaura la dirección original asignada por el fabricante.
Interfaz Intuitiva

Menú interactivo que guía al usuario a través de las opciones disponibles.
Validación de Datos

Asegura que las direcciones MAC ingresadas manualmente tengan un formato válido.
Seguridad

Diseñado para ejecutarse con privilegios administrativos, asegurando cambios efectivos en el sistema.
Requisitos
Sistema Operativo: Windows 10 o superior.
PowerShell: Versión 5.0 o superior.
Permisos de Administrador: El script debe ejecutarse con privilegios elevados.
Cómo Usar
Descargar el Script

Clona este repositorio o descarga el archivo MacManager.ps1.
Ejecutar el Script

Abre PowerShell como administrador.
Navega a la ubicación donde se encuentra el script:
powershell
Copiar código
cd <ruta-del-archivo>
Ejecuta el script:
powershell
Copiar código
.\MacManager.ps1
Seleccionar una Opción del Menú

Sigue las instrucciones del menú interactivo para realizar la operación deseada.
Opciones del Menú
Mostrar interfaces de red disponibles

Lista todas las interfaces de red junto con su estado, dirección MAC y velocidad de conexión.
Ver dirección MAC actual de una interfaz

Solicita el nombre de la interfaz y muestra la dirección MAC configurada actualmente.
Cambiar dirección MAC a una aleatoria

Genera una dirección MAC válida y la aplica automáticamente a la interfaz seleccionada.
Cambiar dirección MAC manualmente

Solicita al usuario ingresar una dirección MAC específica y la aplica a la interfaz seleccionada.
Restaurar dirección MAC predeterminada

Elimina cualquier dirección MAC personalizada y restaura la original del fabricante.
Salir

Cierra el script.
Ejemplo de Uso
Ejemplo: Cambiar la dirección MAC a una aleatoria
Selecciona la opción 3 en el menú.
Ingresa el nombre de la interfaz (por ejemplo, Wi-Fi).
El script generará y aplicará una nueva dirección MAC aleatoria.
plaintext
Copiar código
===============================
     Gestor de MAC Address
===============================
1. Mostrar interfaces de red disponibles
2. Ver dirección MAC actual de una interfaz
3. Cambiar dirección MAC a una aleatoria
4. Cambiar dirección MAC manualmente
5. Restaurar dirección MAC predeterminada
6. Salir
===============================
Seleccione una opción: 3
Ingrese el nombre de la interfaz: Wi-Fi
Generando nueva dirección MAC: 6A-56-0F-D2-82-7D
Deshabilitando la interfaz 'Wi-Fi'...
Cambiando dirección MAC a 6A-56-0F-D2-82-7D...
Habilitando la interfaz 'Wi-Fi'...
Dirección MAC cambiada exitosamente a 6A-56-0F-D2-82-7D
Notas Importantes
Ejecutar como Administrador

El script requiere privilegios elevados para modificar la configuración del adaptador de red.
Validación de MAC Manual

Las direcciones MAC personalizadas deben cumplir con el formato XX-XX-XX-XX-XX-XX y usar valores hexadecimales válidos.
Políticas de Seguridad

En entornos corporativos, las políticas de grupo podrían restringir el acceso al registro o la modificación de direcciones MAC.
Contribuciones
Si deseas colaborar con mejoras, correcciones o nuevas funcionalidades, abre un pull request o crea un issue en este repositorio.

Licencia
Este proyecto está licenciado bajo la MIT License.
