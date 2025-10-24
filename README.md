# Urban.Lunch – Pruebas Exploratorias Móviles  

## Descripción  
Este proyecto documenta una **sesión de pruebas exploratorias** enfocada en evaluar la funcionalidad principal de la aplicación móvil **Urban Lunch**, una plataforma para personalizar comidas de negocios con pedidos combinados de diferentes restaurantes.  

El objetivo fue **verificar la estabilidad y usabilidad del flujo de pedido**, desde la selección del punto de recogida hasta la confirmación y seguimiento del pedido, identificando defectos críticos antes de futuras fases de automatización.  

## Funcionalidades Evaluadas  
1. Selección del punto de recogida  
2. Elección de platillos  
3. Confirmación del pedido  
4. Pantalla de seguimiento de pedidos  
5. Estado de pedido entregado  

## Herramientas y Entorno de Pruebas  
- **Android Studio 2024.3.2** con emulador de dispositivo virtual Android 13.0 ("Tiramisu")  
- **Jira** para documentación y seguimiento de defectos  
- **APK de Urban Lunch (versión de pruebas internas)**  

## Resultados del Sprint de Pruebas  
Durante el primer sprint se identificaron **3 defectos de alta prioridad**, relacionados con la validación del flujo de pedido y la actualización del estado del pedido en la pantalla de seguimiento.  

Todos los defectos fueron registrados y documentados en **Jira**, con evidencia visual y pasos de reproducción para su corrección por parte del equipo de desarrollo.  

### Resumen de Defectos
|  ID Jira   | Severidad | Descripción breve | Estado |
|------------|------------|------------------|---------|
| KAS3RG5S-1 | Alta | Al rotar la pantalla, la selección de platillos que hizo el usuario es eliminada | Abierto |
| KAS3RG5S-2 | Alta | Al rotar la pantalla los pasos ya completados cambian de estado | Abierto |
| KAS3RG5S-3 | Crítica | La aplicación cierra cuando el contador llega a cero en la pantalla "Seguimiento de pedidos" | Abierto |

### Evidencia Visual  
A continuación se muestran capturas de los hallazgos encontrados:
- KAS3RG5S-1
<img width="300" height="635" alt="1-1" src="https://github.com/user-attachments/assets/26a372b0-9598-406e-8001-1083c418bf9c" />
<img width="635" height="300" alt="1-2" src="https://github.com/user-attachments/assets/70aa076c-e09a-4704-a607-10acd8800d03" />
_______________________________________________________________________________________________________________________________________________


- KAS3RG5S-2
<img width="300" height="635" alt="2-1" src="https://github.com/user-attachments/assets/0500f288-e6bd-4a77-a64b-4f3397f5ab83" />
<img width="635" height="300" alt="2-2" src="https://github.com/user-attachments/assets/b93f33f9-74b5-4b52-b4a2-4b44f7079bf1" />
_______________________________________________________________________________________________________________________________________________

- KAS3RG5S-3
🎥 [Ver demostración del error #3 en Google Drive](https://drive.google.com/file/d/1gDfavWpeN1vPr6RK147O1CKe_WaRufVZ/view?usp=sharing)<br>



## Contexto del Proyecto  
**Urban Lunch** busca ofrecer comidas de negocios personalizadas combinando platillos de distintos restaurantes en un solo pedido.  

El flujo principal de usuario es el siguiente:  
1. El usuario selecciona el punto de recogida.  
2. Elige platillos de la lista disponible.  
3. Confirma el pedido.  
4. El sistema coordina la preparación y recogida de los platillos en los restaurantes asociados.  
5. Los pedidos se entregan en el punto de recogida seleccionado en el paso 1.
