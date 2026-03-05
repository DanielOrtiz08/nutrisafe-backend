# 🥗 NutriSafe

**NutriSafe** es una plataforma colaborativa de análisis nutricional y optimización de compra en supermercados.

Permite a los usuarios:

* Subir información nutricional de productos.
* Validar colectivamente etiquetas (modelo tipo Wikipedia).
* Crear perfiles alimenticios personalizados.
* Obtener recomendaciones optimizadas según objetivos y restricciones.
* Priorizar criterios como economía, calidad nutricional, variedad o compra en un solo supermercado.

---

## 🚀 Problema que resuelve

Comprar saludable no es solo leer etiquetas.

Las personas necesitan:

* Comparar productos por macros y micronutrientes.
* Ajustar decisiones según presupuesto.
* Evitar ingredientes no deseados.
* Optimizar su compra según objetivos personales (subir peso, recomposición corporal, dieta baja en azúcar, etc.).

Actualmente esa decisión es manual, lenta y poco sistemática.

NutriSafe automatiza y optimatiza ese proceso.

---

## 🧠 Enfoque Técnico

### Arquitectura

* Backend: **Spring Boot (Monolito modular)**
* Base de datos: PostgreSQL
* Despliegue: Microsoft Azure
* Arquitectura preparada para futura migración a microservicios
* API RESTful + soporte para múltiples protocolos

### Protocolos de comunicación

* HTTP/REST
* WebSockets (para validaciones colaborativas en tiempo real)
* Posible integración futura con gRPC

### Infraestructura

* Azure App Services
* Azure Database for PostgreSQL
* Azure Blob Storage (imágenes de etiquetas)
* CI/CD preparado para GitHub Actions

---

## 🏗️ Modelo Colaborativo (Descentralización Lógica)

NutriSafe implementa un sistema de validación comunitaria:

1. Un usuario sube un producto.
2. Otros usuarios pueden:

   * Confirmar datos.
   * Reportar inconsistencias.
   * Proponer correcciones.
3. Se aplica un sistema de reputación.
4. El producto obtiene un nivel de confiabilidad.

Inspiración conceptual:

* Wikipedia (validación colectiva)
* StackOverflow (reputación)
* Sistemas distribuidos con consenso ligero

---

## ⚙️ Motor de Optimización

El núcleo diferencial del sistema es el motor de optimización.

### Funcionalidades previstas:

* Optimización multicriterio:

  * Precio
  * Calidad nutricional
  * Densidad proteica
  * Nivel de procesamiento
  * Restricciones alimentarias

* Algoritmos:

  * Búsqueda heurística
  * Optimización por scoring ponderado
  * Posible implementación futura de algoritmos tipo:

    * Knapsack Problem
    * Dijkstra (para rutas óptimas entre supermercados)
    * Algoritmos genéticos (fase avanzada)

---

## 👤 Perfil Nutricional Inteligente

Cada usuario define:

* Peso
* Altura
* Objetivo (subir peso, perder grasa, recomposición, mantenimiento)
* Restricciones (lactosa, gluten, ultraprocesados, etc.)
* Presupuesto

El sistema:

* Calcula requerimientos calóricos y de macronutrientes.
* Genera recomendaciones personalizadas.
* Prioriza según preferencias del usuario.

---

## 📊 Futuras Integraciones

* Machine Learning para:

  * Recomendaciones personalizadas
  * Predicción de preferencias
  * Detección automática de inconsistencias en etiquetas
* OCR para escaneo automático de productos
* Aplicación móvil multiplataforma

---

## 🛠️ Stack Tecnológico

* Java 21
* Spring Boot
* Spring Security
* JPA / Hibernate
* PostgreSQL
* Docker
* Azure
* GitHub Actions

---

## 📦 Estructura del Proyecto (Monolito Modular)

```
nutrisafe/
 ├── user-module
 ├── product-module
 ├── validation-module
 ├── optimization-module
 ├── recommendation-module
 └── infrastructure
```

Cada módulo es desacoplado internamente para facilitar futura separación en microservicios.

---

## 🔐 Seguridad

* Autenticación JWT
* Roles:

  * Usuario
  * Validador
  * Administrador
* Rate limiting
* Validación de datos nutricionales

---

## 🎯 Estado del Proyecto

En fase de desarrollo.

Objetivo actual:

* Construir MVP funcional con:

  * Registro de usuarios
  * Subida de productos
  * Sistema básico de validación
  * Recomendación por scoring simple

---

## 🤝 Contribuciones

Las contribuciones son bienvenidas.

Próximamente se publicará guía de contribución y estándares de código.

