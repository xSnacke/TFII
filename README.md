# 👟 Flow Zapas - Sistema Gestor de Stock, Facturación y Ventas

## 📌 Descripción del Proyecto
*Flow Zapas* es un sistema integral de gestión comercial desarrollado para optimizar la administración de inventario, ventas y facturación en negocios del rubro calzado e indumentaria.

El mayor desafío técnico de este dominio radica en la *gestión multidimensional de inventario* (un mismo modelo se fracciona en múltiples variantes por talle, color y SKU único), requiriendo un control de stock atómico para evitar inconsistencias tanto en venta física como digital.

---

## 🏗️ Arquitectura y Tecnologías

El sistema está desarrollado en *.NET 8 (C#)* aplicando principios de *Clean Architecture* (Arquitectura en Capas) para garantizar mantenibilidad, testabilidad y escalabilidad:

1. *FlowZapas.Domain*: Entidades core del negocio (Product, ProductVariant, Sale, Invoice, Customer) e interfaces base.
2. *FlowZapas.Data: Persistencia relacional mediante **Entity Framework Core, implementación del patrón *Repository y Unit of Work.
3. *FlowZapas.Business*: Lógica de negocio, validaciones transaccionales y transferencia de datos mediante DTOs.
4. *FlowZapas.Api*: Capa de presentación RESTful con ASP.NET Core y documentación interactiva mediante Swagger.

---

## 🛠️ Patrones de Diseño Aplicados
- *Clean Architecture / N-Tier:* Separación estricta de responsabilidades.
- *Repository & Unit of Work:* Abstracción de la capa de datos y control atómico de transacciones.
- *Strategy Pattern:* Implementación flexible de métodos de pago (Efectivo, Transferencia, Posnet) y políticas de facturación.
- *DTOs (Data Transfer Objects):* Aislamiento entre el modelo de dominio y la capa de exposición API.

---

## 🚀 Módulos del Sistema
- [x] *Gestión de Stock y Calzado:* Control por modelo, talle, color y SKU con alertas de stock mínimo.
- [x] *Módulo de Ventas:* Registro transaccional de operaciones con validación previa de stock.
- [x] *Módulo de Facturación:* Emisión de comprobantes y trazabilidad de historial de caja.
- [x] *Reportes:* Estadísticas de modelos más vendidos y métricas comerciales.

---

## 👥 Integrantes del Equipo
- Trabajo Integrador / Colaborativo de Programación y Metodologías.
