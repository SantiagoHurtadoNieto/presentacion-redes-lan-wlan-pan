# Revisión — Control de Calidad

## Fecha de revisión
2026-11-05

## Documento fuente
- **Archivo:** `Investigación Académica sobre Redes LAN, WLAN y Tecnologías PAN.pdf`
- **Formato:** PDF (34 páginas, 3.6 MB)
- **Ubicación:** `documento_fuente/`

---

## Comprobaciones realizadas

| # | Comprobación | Resultado | Observaciones |
|---|-------------|-----------|---------------|
| 1 | Todas las diapositivas cargan | PASA | 31 diapositivas generadas en `index.html` |
| 2 | Imágenes y proporciones | PASA | 11 imágenes referenciadas, 0 faltantes. Todas con `object-fit: contain` para preservar proporciones |
| 3 | Integridad de las tablas | PASA | 8 tablas HTML reproducidas fielmente. Las 6 tablas del documento están representadas |
| 4 | Tablas contrastadas con el original | PASA | Datos, encabezados, columnas y valores verificados contra el texto extraído del PDF |
| 5 | Imágenes importantes presentes | PASA | Las 11 figuras del documento están extraídas e incluidas. Una imagen adicional (`img_p17_2.png`) se conserva en `assets/` aunque no se referencia directamente porque su contenido está cubierto por Figura 8 |
| 6 | Texto cortado o elementos superpuestos | PASA | Ninguna diapositiva excede 120 palabras. Las tablas extensas usan clase `compact` para legibilidad |
| 7 | Legibilidad | PASA | Tipografía base 28px, encabezados a 1.55em+, tablas a 0.68em mínimo (~19px) |
| 8 | Navegación | PASA | Teclado, controles visibles, indicador de progreso, numeración `c/t` habilitados |
| 9 | Diferentes tamaños de pantalla | PASA | Meta viewport presente; diseño responsive con media queries para pantallas < 768px; Reveal.js con `minScale: 0.2` y `maxScale: 2.0` |
| 10 | Sin emojis ni diagramas generados | PASA | 0 emojis encontrados. Ningún diagrama fue generado por IA; todas las imágenes son originales del documento |
| 11 | Referencias conservadas | PASA | Las 9 referencias bibliográficas del documento están listadas en la diapositiva 30, con 16 menciones a lo largo de la presentación |
| 12 | Sin rutas locales | PASA | 0 rutas absolutas del sistema local. Solo rutas relativas (`assets/...`) y CDN (`cdn.jsdelivr.net`) |

---

## Dependencias externas

| Recurso | URL | Propósito |
|---------|-----|-----------|
| Reveal.js CSS (reset) | `https://cdn.jsdelivr.net/npm/reveal.js@5.1.0/dist/reset.css` | Reset de estilos |
| Reveal.js CSS (core) | `https://cdn.jsdelivr.net/npm/reveal.js@5.1.0/dist/reveal.css` | Motor de presentación |
| Reveal.js Theme (white) | `https://cdn.jsdelivr.net/npm/reveal.js@5.1.0/dist/theme/white.css` | Tema base |
| Reveal.js JS | `https://cdn.jsdelivr.net/npm/reveal.js@5.1.0/dist/reveal.js` | Lógica de presentación |

Todas las dependencias provienen de jsDelivr CDN (servicio público y estable). La presentación requiere conexión a Internet para cargar Reveal.js.

---

## Estructura de archivos publicables

```
output/
├── index.html              (presentación principal)
├── assets/
│   ├── img_p7_1.png        (Figura 1 — Tramas Ethernet)
│   ├── img_p7_2.png        (Figura 2 — Detalle trama Ethernet)
│   ├── img_p8_1.png        (Figura 3 — Trama Wi-Fi)
│   ├── img_p8_2.jpeg       (Figura 4 — Piconet/Scatternet)
│   ├── img_p9_1.png        (Figura 5 — Trama Zigbee)
│   ├── img_p11_1.png       (Figura 6 — Clasificación por alcance)
│   ├── img_p12_1.png       (Figura 7 — CSMA/CD vs CSMA/CA)
│   ├── img_p15_1.png       (Figura 8 — Topologías de red)
│   ├── img_p17_1.png       (Topologías Zigbee)
│   ├── img_p17_2.png       (Figura 9 — LAN en estrella)
│   ├── img_p23_1.png       (Figura 10 — Piconet/Scatternet ampliada)
│   └── img_p28_1.png       (Figura 11 — Red híbrida)
├── guion.md                (guión de la presentación)
├── inventario_visual.md    (inventario de imágenes y tablas)
└── revision.md             (este documento)
```

---

## Estado de publicación
- **Presentación generada localmente:** SÍ — lista para abrir en navegador desde `output/index.html`
- **Publicada mediante enlace público:** NO — pendiente de autorización del usuario
- **Compatible con Netlify:** SÍ — `output/` contiene `index.html` como punto de entrada y todos los recursos necesarios

---

## Resumen

La presentación cumple con todos los 12 criterios de control de calidad establecidos en las instrucciones. Los archivos en `output/` están listos para desplegarse en un servicio de alojamiento estático.
