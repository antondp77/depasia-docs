# DEPASIA DOCS — MASTER CONTEXT V1

## 1. Objetivo
DEPASIA DOCS es una aplicación interna de DEPASIA para preparar, revisar, aprobar y generar documentos oficiales.

La primera versión debe ser pequeña, clara y fácil de mantener.

### Primera meta
**Crear Presupuesto → completar datos → vista previa → generar PDF**

No construir todo el sistema documental desde el comienzo.

## 2. Estado actual

**Todavía NO existe ningún template visual definitivo.**

Esto es una decisión importante para el desarrollo.

No inventar ni asumir el diseño final del Presupuesto.

Antes de implementar el PDF definitivo debemos crear y aprobar la primera plantilla visual maestra de Presupuesto.

### Orden correcto
1. Definir plantilla visual de Presupuesto.
2. Aprobar diseño.
3. Convertir plantilla en código.
4. Crear formulario de datos.
5. Generar vista previa.
6. Generar PDF.
7. Validar.
8. Reutilizar la arquitectura para otros documentos.

## 3. Principio de diseño
Separar:
- Datos.
- Plantilla.
- Documento.
- Revisión.
- Aprobación.
- PDF.

No mezclar lógica comercial con diseño visual.

## 4. Primera plantilla

El primer documento será **Presupuesto**.

La plantilla deberá contemplar, como mínimo:
- Identidad DEPASIA.
- Logo oficial cuando estén disponibles los assets maestros.
- Nombre del documento.
- Número de presupuesto.
- Fecha.
- Datos del cliente.
- Descripción del servicio.
- Alcance.
- Importe.
- Moneda.
- Condiciones.
- Validez.
- Observaciones.
- Datos de contacto.
- Pie institucional.

Los campos exactos deberán definirse al diseñar la plantilla.

## 5. Identidad DEPASIA
Tagline: **Sistemas que hacen crecer tu negocio**

Colores:
- Blue: #2563EB
- Violet: #7C3AED
- Cyan: #0686D4

Gradiente: Cyan → Blue → Violet

Neutros:
- #0F172A
- #1E293B
- #334155
- #64748B
- #94A3B8
- #F8FAFC

Tipografía: **Inter**

El logo oficial está definido como referencia, pero los assets maestros editables todavía deben obtenerse/generarse. No recrear ni modificar el logo arbitrariamente.

## 6. Usuarios

### Founder / Director
Tonio.

Puede crear, editar, aprobar, generar PDF y gestionar plantillas.

### Operador / Agente
En el futuro podrá crear, consultar, preparar y actualizar borradores y solicitar aprobación.

No debe aprobar su propia acción cuando exista separación de aprobación ni modificar precios/condiciones sin autorización.

## 7. Agentes

DEPASIA DOCS no debe depender de Grok.

Grok será inicialmente el operador principal de DEPASIA, pero la aplicación debe ser independiente del proveedor de IA.

En el futuro podrá utilizarse desde:
- Grok
- Agentes propios de DEPASIA OS
- Hermes
- GPT
- Otros agentes

Capacidades futuras:
- create_document
- preview_document
- update_document
- get_document
- generate_pdf
- list_templates

Los agentes no deben acceder directamente a la base de datos para ejecutar estas operaciones.

## 8. Flujo humano inicial

```text
Usuario
  ↓
Seleccionar Presupuesto
  ↓
Completar datos
  ↓
Guardar borrador
  ↓
Vista previa
  ↓
Revisar
  ↓
Aprobar
  ↓
Generar PDF
```

## 9. Flujo futuro con Grok

```text
Tonio
  ↓
Grok
  ↓
Consulta información administrativa
  ↓
Prepara datos
  ↓
DEPASIA DOCS
  ↓
Valida
  ↓
Crea documento
  ↓
Solicita aprobación cuando corresponda
  ↓
Genera PDF
```

Grok no debe inventar datos.

## 10. Estados

Estados documentales previstos:
- Borrador
- En revisión
- Aprobado
- Enviado
- Firmado
- Finalizado
- Archivado

El MVP puede comenzar con:
- Borrador
- En revisión
- Aprobado
- Generado

## 11. Numeración

Usar numeración humana:
**Presupuesto #001**

Los identificadores técnicos pueden existir internamente, pero no deben molestar al usuario.

## 12. Reglas comerciales

Nunca inventar:
- precios
- descuentos
- impuestos
- condiciones
- plazos
- datos de clientes
- servicios
- compromisos

Las operaciones matemáticas sí pueden ser automáticas.

## 13. Stack

Preferido:
- Next.js
- TypeScript
- Tailwind CSS
- shadcn/ui
- Supabase cuando realmente sea necesario
- Vercel
- GitHub

No agregar tecnologías innecesarias.
No crear microservicios.
No construir un sistema complejo de templates.

## 14. Persistencia

La arquitectura debe permitir guardar documentos y versiones.

Si para validar el primer flujo no hace falta una base de datos completa, puede comenzar con una implementación simple.

No construir una base de datos compleja antes de conocer las necesidades reales.

## 15. PDF

El PDF debe representar fielmente la plantilla aprobada y ser:
- profesional
- legible
- consistente
- imprimible
- usable desde computadora y celular

Preview y PDF deben mantener la misma estructura visual.

## 16. Fuera del alcance inicial

No construir todavía:
- firma electrónica
- facturación
- portal de clientes
- CRM
- WhatsApp API
- email automático
- editor visual de templates
- todos los tipos de documentos
- sistema avanzado de permisos
- sistema avanzado de agentes
- DEPASIA OS
- microservicios

## 17. Criterio de éxito

Tonio debe poder:
1. Abrir DEPASIA DOCS.
2. Crear un Presupuesto.
3. Completar los datos.
4. Guardarlo como borrador.
5. Ver una vista previa profesional.
6. Revisarlo.
7. Aprobarlo.
8. Generar un PDF.
9. Obtener un documento consistente con DEPASIA.

## 18. Regla para Cursor

Antes de programar una parte todavía no definida, marcarla como pendiente.

No inventar decisiones de producto.
No sobreingenierizar.
No agregar funcionalidades porque parezcan útiles.
Primero implementar lo definido.
