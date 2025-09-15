# Historia de Usuario 5: Gestión de Estatus de Herramentales en Tiempo Real

## Como
Técnico

## Quiero
Ver la pantalla de seguimiento y cambiar el estatus de cada herramental en un pedido, con actualización en tiempo real

## Para
Mantener informado al equipo sobre el estado actual del proceso de fabricación y gestionar eficientemente los herramentales

## Criterios de Aceptación
1. El técnico debe poder acceder a una pantalla de seguimiento donde se muestren todos los pedidos activos
2. Para cada pedido, se deben visualizar los herramentales asociados y su estado actual
3. El técnico debe poder cambiar el estatus de cada herramental entre las siguientes opciones: disponible, montándose, uso, en paro, en mantenimiento, fin de uso y en cambio
4. Cuando se cambie el estatus a "en cambio", el sistema debe mostrar automáticamente todos los herramentales compatibles que estén disponibles
5. El técnico debe poder seleccionar un herramental de reemplazo de la lista de compatibles
6. La pantalla de seguimiento debe actualizarse en tiempo real para todos los usuarios sin necesidad de refrescar la página (sin F5)
7. Debe existir un registro histórico de los cambios de estatus para cada herramental en un pedido

## Preguntas adicionales
- ¿Se requiere registrar quién realizó cada cambio de estatus y cuándo?
- ¿Es necesario agregar comentarios al cambiar el estatus de un herramental?
- ¿Deben existir restricciones para cambiar de ciertos estatus a otros (por ejemplo, no se puede pasar directamente de "disponible" a "fin de uso")?
- ¿Se necesitan notificaciones cuando ocurren ciertos cambios de estatus?
- ¿Cuál es el flujo de trabajo esperado entre los diferentes estatus?
```