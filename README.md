# Diseño de Red Empresarial para Entorno Industrial  
**Caso de Estudio Académico – Infraestructura de Telecomunicaciones**

## Autores

> Tomás Lopera

> Pedro Sierra

## Descripción del Proyecto

Este proyecto presenta el diseño completo de una infraestructura de red empresarial para una organización manufacturera compuesta por:

- 2 edificios interconectados
- 3 pisos administrativos
- 1 planta de producción industrial
- Más de 200 puntos de red
- Maquinaria industrial, cámaras IP y laboratorios TIC

El diseño contempla infraestructura física, topología lógica, direccionamiento IP y segmentación por áreas funcionales.

## Objetivos

- Diseñar un sistema de cableado estructurado bajo estándares internacionales.
- Garantizar escalabilidad, organización y facilidad de mantenimiento.
- Optimizar el direccionamiento IP reduciendo desperdicio mediante CIDR.
- Soportar entornos administrativos e industriales de alta demanda.

## Arquitectura Física

### Cableado Horizontal
- UTP Categoría 6a (10 Gbps, soporte PoE+)
- Topología estrella
- Máximo 90 metros por tramo (ANSI/TIA-568-D.2)

### Cableado Vertical (Backbone)
- Fibra óptica OM3
- Velocidades entre 40–100 Gbps
- Topología estrella jerarquizada

### Infraestructura de Telecomunicaciones
- Closets por piso con gabinetes 42U
- Switches de 24 y 48 puertos
- Access Points estratégicamente ubicados
- Separación de canalizaciones según normativa ANSI/TIA-569-D

## Arquitectura Lógica

- Segmentación por áreas: Administración, TIC, Compras, Finanzas, Marketing y Producción.
- VLANs independientes por departamento.
- Direccionamiento IP con análisis comparativo:
  - Enfoque con clase
  - Enfoque sin clase (CIDR) → menor desperdicio de direcciones IP

El diseño sin clase reduce significativamente el desperdicio de direcciones y mejora la escalabilidad.

## Entorno Industrial

La planta de producción incluye:

- 70 equipos industriales (doble interfaz de red)
- 26 cámaras IP
- Estaciones de control de banda
- NAS para respaldo de datos
- Access Points de cobertura extendida

Se implementa segmentación para aislar tráfico industrial, administrativo y de videovigilancia.
