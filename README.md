# 💰 Mis Finanzas

Aplicación personal de finanzas: ingresos, gastos, ahorro, inversiones, patrimonio, fondos (metas) y costos del negocio. Todo en un solo archivo, sin servidores — tus datos viven **solo en tu dispositivo**.

## ✨ Características

- **Mes**: balance del mes, anillo de disponible, cascada de a dónde se va el ingreso, movimientos (con edición y retiros de ahorro).
- **Plan**: distribución del ingreso (% o monto fijo en USD/MXN), plan vs. real, recurrentes mensuales con botón "aplicar al mes".
- **Cartera**: patrimonio neto, balance general (activos/pasivos), bancos, bienes, bienes raíces con hipoteca, deudas, cuentas de inversión y posiciones (con alerta de CETES vencidos).
- **Fondos**: metas de ahorro con proyección de fecha y botón "Realizar" al completarlas.
- **Negocio**: costos operativos con opción de incluirlos en la proyección.
- **Futuro**: proyección de flujo libre a 12 meses.
- **Bilingüe**: español / English (Plan → Ajustes → Idioma).
- **Respaldo**: exporta/restaura todos tus datos en JSON (Plan → Respaldo de datos) y CSV para Excel.
- **PWA**: instalable como app con ícono propio y funciona sin internet.

## 📱 Instalarla en el iPhone

1. Publica el repositorio con GitHub Pages (una sola vez):
   - En GitHub: **Settings → Pages → Source: Deploy from a branch → Branch: `main` / (root) → Save**.
   - Tu app quedará en `https://<tu-usuario>.github.io/app-mis-finanzas/`.
2. Abre esa URL en **Safari** en el iPhone.
3. Toca **Compartir → Agregar a pantalla de inicio**.
4. Listo: aparece con el logo dorado/verde como una app más, a pantalla completa y funcionando offline.

> 💡 **Haz respaldos**: Safari puede borrar datos de sitios que no visitas en semanas. Entra a **Plan → Respaldar (JSON)** de vez en cuando y guarda el archivo en iCloud/Archivos. Con **Restaurar** recuperas todo en cualquier dispositivo.

## 🧠 Mi Conocimiento

En este mismo repositorio vive una segunda app: **[Mi Conocimiento](conocimiento/)**, un
cuaderno de estudio con memoria: notas de tres preguntas (qué aprendí, el comando o ejemplo,
cómo lo practiqué), búsqueda instantánea sobre tus propias palabras, repaso espaciado que te
pregunta antes de que olvides, y rutas de estudio opcionales.

Se instala aparte, con su propio ícono:
`https://<tu-usuario>.github.io/app-mis-finanzas/conocimiento/`

## 🗂 Estructura

```
index.html        ← Mis Finanzas: la app completa (HTML + CSS + JS)
manifest.json     ← manifiesto PWA (nombre, ícono, colores)
sw.js             ← service worker (funciona offline)
icons/            ← logo e íconos de la app
conocimiento/     ← Mi Conocimiento: la app de notas (misma estructura, datos aparte)
```

`MIS FINANZAS/misfinanzas.html` es la versión anterior; se conserva como referencia y puede borrarse cuando quieras.

## 🔒 Privacidad

Estas apps se pueden compartir con toda confianza: **compartes el enlace, nunca tus datos.**

- Todos los datos (movimientos, patrimonio, notas) viven **únicamente en el navegador de cada
  dispositivo**. No hay servidor, no hay cuentas y las apps no hacen ninguna llamada a internet.
- Cada persona que abre el enlace empieza con su propia app vacía. Nadie —ni siquiera el autor—
  puede ver los datos de otra persona.
- Por lo mismo, **el respaldo es responsabilidad de cada quien**: el navegador puede borrar los
  datos de sitios que no visitas en semanas. Descarga tu respaldo JSON con regularidad y guárdalo
  en iCloud/Drive.
- El PIN de Mis Finanzas es un candado de pantalla, no un cifrado: protege de miradas casuales,
  no sustituye la seguridad de tu teléfono.

## 📄 Licencia

Código bajo [licencia MIT](LICENSE): puedes usarlo, copiarlo y adaptarlo libremente, sin garantía.

