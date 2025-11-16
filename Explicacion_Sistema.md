# Sistema de Venta de Boletos en Físico

## Descripción General

El Sistema de Venta de Boletos en Físico es una solución que permite a los vendedores gestionar de manera eficiente el proceso completo de venta de boletos para películas. Este sistema proporciona una interfaz intuitiva que guía al vendedor a través de cada etapa de la transacción, desde la selección de la película hasta la emisión del boleto final.

---

## Nivel 0: Proceso General

El Nivel 0 representa el flujo principal del sistema, que constituye el núcleo del negocio de venta de boletos. Este nivel desglosa el proceso en cuatro etapas fundamentales que se ejecutan de manera secuencial:

### 1. **Seleccionar Película**
El vendedor inicia el proceso seleccionando la película que desea el cliente. Esta acción es fundamental pues establece la base para todas las decisiones posteriores. Sin una película seleccionada, no es posible avanzar en el proceso de venta.

### 2. **Seleccionar Horario**
Una vez definida la película, el sistema requiere que el vendedor seleccione el horario de proyección disponible. Esta decisión es crítica pues garantiza que el cliente obtenga el boleto para la sesión que desea asistir.

### 3. **Seleccionar Asiento**
Después de confirmar el horario, el vendedor procede a seleccionar el asiento específico en la sala de cine. Esta etapa asegura la reserva temporal del lugar para evitar conflictos de doble venta y proporciona una experiencia personalizada al cliente.

### 4. **Realizar Pago**
Finalmente, el sistema requiere completar la transacción económica. En esta etapa se registran los datos del cliente, se selecciona el método de pago, se aplican promociones si aplican, y se calcula el total final antes de emitir el boleto.

---

## Nivel 1: Casos de Uso Detallados

El Nivel 1 desglosa cada uno de los casos de uso del Nivel 0, proporcionando una visión más granular de los procesos específicos que el sistema debe soportar.

### **Nivel 1.1: Detalles de Seleccionar Película**

Este nivel detalla cómo el vendedor interactúa con el catálogo de películas disponibles:

- **Listar Películas Disponibles**: El sistema presenta automáticamente todas las películas en cartelera. Esta funcionalidad es esencial y se ejecuta siempre, proporcionando al vendedor una vista completa del inventario de películas.

- **Buscar Película por Nombre o Género**: El sistema ofrece al vendedor la capacidad de buscar películas específicas utilizando criterios como el nombre o género. Esta función es opcional pero mejora significativamente la eficiencia cuando se busca una película particular sin necesidad de revisar toda la lista.

- **Ver Detalles de Película**: El vendedor puede acceder a información ampliada sobre cada película, incluyendo sinopsis, duración, calificación, director y otros datos relevantes. Esta función es opcional pero proporciona al vendedor información valiosa para asesorar mejor al cliente sobre su elección.

---

### **Nivel 1.2: Detalles de Seleccionar Horario**

Este nivel especifica cómo el sistema gestiona la selección de horarios disponibles:

- **Mostrar Horarios Disponibles**: El sistema presenta todos los horarios de proyección disponibles para la película seleccionada. Esta funcionalidad es obligatoria y forma la base para que el vendedor pueda ofrecerle opciones al cliente.

- **Filtrar Horarios por Rango**: El vendedor puede filtrar los horarios disponibles según un rango de tiempo específico que sea conveniente para el cliente. Esta función es opcional pero resulta práctica cuando el cliente tiene restricciones horarias.

- **Ver Capacidad Restante**: El sistema muestra cuántos asientos disponibles quedan en cada horario. Esta funcionalidad es opcional pero es crucial para que el vendedor informe al cliente sobre la disponibilidad de la sesión antes de hacer la reserva.

---

### **Nivel 1.3: Detalles de Seleccionar Asiento**

Este nivel describe cómo el sistema maneja la selección de asientos:

- **Mostrar Mapa de Asientos**: El sistema presenta una visualización del mapa de la sala con los asientos disponibles e indisponibles. Esta funcionalidad es obligatoria pues permite al vendedor y al cliente ver la distribución física de la sala.

- **Reservar Asiento Temporalmente**: El sistema reserva el asiento seleccionado de manera temporal para evitar que otro vendedor venda el mismo asiento simultáneamente. Esta funcionalidad es obligatoria y crítica para mantener la integridad del inventario.

- **Cambiar Selección de Asiento**: El vendedor puede modificar la selección de asiento si el cliente cambia de opinión. Esta función es opcional pero proporciona flexibilidad durante el proceso de venta.

---

### **Nivel 1.4: Detalles de Realizar Pago**

Este nivel detalla los pasos necesarios para completar la transacción financiera:

- **Ingresar Datos del Cliente**: El sistema registra la información personal del cliente, incluyendo nombre, contacto y datos de identificación. Esta funcionalidad es obligatoria para la emisión del boleto.

- **Seleccionar Método de Pago**: El vendedor selecciona el medio de pago que utilizará el cliente, ya sea efectivo, tarjeta de crédito, tarjeta de débito u otros métodos disponibles. Esta funcionalidad es obligatoria para procesar la transacción.

- **Aplicar Descuento**: El sistema permite aplicar promociones, descuentos por cantidad o cupones especiales si aplican a la compra. Esta funcionalidad es opcional pues no todas las transacciones incluyen descuentos.

- **Calcular Total**: El sistema calcula el monto final a pagar considerando el precio del boleto, cantidad de boletos y descuentos aplicados. Esta funcionalidad es obligatoria para determinar el importe que el cliente debe pagar.

- **Imprimir Boleto**: El sistema emite el boleto físico con toda la información relevante (película, horario, asiento, fecha, precio). Esta funcionalidad es obligatoria pues representa el producto final que el cliente recibe.

---

## Conclusión

El Sistema de Venta de Boletos en Físico está estructurado de manera jerárquica donde el Nivel 0 establece el flujo general de cuatro pasos principales, y el Nivel 1 desglosa cada uno de estos pasos en funcionalidades específicas. Esta arquitectura permite que el sistema sea flexible, mantenible y escalable, proporcionando a los vendedores las herramientas necesarias para gestionar eficientemente la venta de boletos mientras garantiza una experiencia satisfactoria para los clientes.
