# DEPASIA DOCS — AGENTS.md

## Rol
Sos el agente de desarrollo de DEPASIA DOCS.

Tu objetivo es implementar el producto de forma simple, estable y mantenible.

## Antes de modificar código
1. Leer `MASTER_CONTEXT.md`.
2. Revisar la estructura existente.
3. Identificar qué parte se está modificando.
4. No cambiar decisiones de producto sin autorización.

## Regla crítica: templates

**El template de Presupuesto todavía NO existe.**

No inventar el diseño final del documento.

Si una tarea depende del diseño visual definitivo:
- marcar la dependencia;
- preparar la estructura técnica necesaria;
- no fijar arbitrariamente posiciones, bloques o textos que todavía no fueron aprobados.

## Desarrollo

Preferir:
- componentes simples;
- funciones pequeñas;
- nombres claros;
- TypeScript;
- reutilización razonable;
- validaciones claras.

Evitar:
- abstracciones prematuras;
- patrones complejos sin necesidad;
- microservicios;
- dependencias innecesarias;
- sistemas de plugins;
- editor visual de templates.

## Arquitectura

Mantener separadas estas responsabilidades:

```text
Datos
 ↓
Modelo de documento
 ↓
Template
 ↓
Preview
 ↓
PDF
```

## IA y agentes

No asumir que Grok forma parte del núcleo técnico.

La aplicación debe funcionar sin una IA.

Las futuras integraciones con Grok, Hermes o agentes propios deben utilizar capacidades controladas.

## Validación

Nunca permitir que datos críticos faltantes generen un documento aparentemente terminado.

Nunca inventar precios, descuentos, impuestos, condiciones, fechas o datos de clientes.

## Prioridad actual

**Presupuesto → Preview → PDF**

Después de validar este flujo se continuará con los demás documentos.

## Forma de trabajo

Implementar en pasos pequeños.

Después de cada bloque:
1. verificar que compila;
2. revisar errores;
3. probar el flujo;
4. documentar decisiones nuevas;
5. continuar.

Si aparece una decisión no definida, detenerse antes de asumirla.
