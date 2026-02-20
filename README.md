# G5-Solutions-S.A.S

# Sistema de Inventarios - G5 Solutions S.A.S

## 📌 Descripción del Proyecto
Este proyecto fue creado como parte de la práctica de **Calidad en el Servicio de Software**.  
El objetivo principal es desarrollar un **Sistema de Inventarios Escolar** que permita gestionar de manera eficiente las entradas y salidas de productos, garantizando control, trazabilidad y facilidad de uso.

## ⚙️ Cómo se creó
- Se utilizó **HTML, CSS y JavaScript** para la construcción de la interfaz y la lógica básica.  
- El proyecto fue gestionado en **GitHub**, con despliegue en **GitHub Pages** para acceso público.  
- Se aplicaron metodologías de **pruebas de software** (casos positivos, negativos y de límite) para validar la calidad del sistema.  
- Se documentaron los casos de prueba en tablas y matrices, siguiendo buenas prácticas de QA.

## 🚀 Funcionalidades principales
- **Gestión de Entradas**: Registrar productos que ingresan al inventario con cantidad y descripción.  
- **Gestión de Salidas**: Registrar productos que salen del inventario, validando stock disponible.  
- **Control de Stock**: Actualización automática de cantidades en tiempo real.  
- **Mensajes de Validación**: Confirmaciones y errores claros (ej. “Stock insuficiente”, “Producto no encontrado”).  
- **Interfaz amigable**: Navegación sencilla y visual para usuarios no técnicos.  
- **Pruebas de Calidad**: Casos de prueba documentados para asegurar confiabilidad y robustez.

## 📂 Estructura del Proyecto
- `/index.html` → Página principal del sistema.  
- `/css/` → Estilos visuales del sistema.  
- `/js/` → Lógica de validación y gestión de inventario.  
- `/docs/` → Documentación y tablas de casos de prueba.  

## 🧪 Pruebas de Calidad
Se diseñaron y ejecutaron matrices de prueba que incluyen:
- Casos positivos (operaciones correctas).  
- Casos negativos (errores esperados).  
- Casos límite (valores extremos).  
- Validaciones de datos incompletos y formatos inválidos.  

## ▶️ Ejemplo de Uso Paso a Paso
1. **Registrar una entrada**  
   - Selecciona el módulo **Entradas**.  
   - Ingresa el producto: *“Laptop Dell”*.  
   - Ingresa la cantidad: *10*.  
   - Haz clic en **Registrar**.  
   - ✅ El sistema confirma: *“Entrada registrada exitosamente”*.  

2. **Registrar una salida**  
   - Selecciona el módulo **Salidas**.  
   - Ingresa el producto: *“Laptop Dell”*.  
   - Ingresa la cantidad: *5*.  
   - Haz clic en **Registrar**.  
   - ✅ El sistema confirma: *“Salida registrada exitosamente”*.  
   - El stock se actualiza automáticamente: ahora quedan *5 unidades*.  

3. **Validación de error**  
   - Intenta registrar salida de *“Laptop Dell”* con cantidad *20*.  
   - ❌ El sistema muestra: *“Stock insuficiente”*.  
   - El registro no se guarda y el stock permanece igual.  

## 🔄 Diagrama de Flujo (Entradas y Salidas)

```mermaid
flowchart TD
    A[Inicio] --> B{Seleccionar módulo}
    B -->|Entradas| C[Ingresar producto y cantidad]
    B -->|Salidas| D[Ingresar producto y cantidad]
    C --> E[Validar datos]
    D --> E[Validar datos]
    E -->|Datos válidos| F[Actualizar stock]
    E -->|Datos inválidos| G[Mostrar mensaje de error]
    F --> H[Confirmar operación]
    G --> H
    H --> I[Fin]

👥 Autores
Proyecto desarrollado por Braynel en el marco de Plataformas Tecnologicas.

