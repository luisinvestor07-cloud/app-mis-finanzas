# 🧠 Mi Conocimiento

Memoria personal de aprendizaje. No es una app para "tomar notas": es para **conservar,
recuperar y aplicar** lo que estudias. Olvidar una definición al mes es normal — lo que
importa es encontrarla en segundos y saber qué hacer con ella.

Vive en el mismo repositorio que Mis Finanzas, pero es una app aparte: se instala con su
propio ícono y sus datos son independientes.

## Las cuatro ideas que la sostienen

**1. Notas pequeñas y conectadas.** En vez de un documento gigante sobre el balance general,
una nota por concepto: *activo corriente*, *capital de trabajo*, *razón corriente*. Cada una
se enlaza con las demás, así que llegas al mismo conocimiento por varios caminos.

**2. Conocimiento y aplicación son notas distintas.**

| 📘 Conocimiento | 🛠️ Aplicación |
|---|---|
| Qué es el capital de trabajo | Cómo calcularlo e interpretarlo |
| Qué es la deuda financiera | Cómo detectar un endeudamiento peligroso |
| Qué es la liquidez | Cómo comparar la liquidez de dos compañías |

Las de conocimiento explican **qué significa**. Las de aplicación son listas de verificación:
te dicen **qué hacer** cuando tienes el documento enfrente. El botón *Crear la nota par*
genera la contraparte y la deja conectada.

**3. Captura sin fricción.** Título y una línea con tus palabras bastan para guardar. Los
demás campos —clasificación, fórmulas, ejemplo, errores, fuentes— se llenan después, cuando
los tengas. Una plantilla que exige diez campos por nota mata el hábito en dos semanas.

**4. Búsqueda instantánea sobre tus propias palabras.** Local, sin internet. Entiende
preguntas escritas de corrido: *«¿qué fórmula usé para capital de trabajo?»*,
*«¿dónde escribí sobre inventarios?»*.

## Cómo se usa

La app es un cuaderno de tres pestañas:

- **📒 Notas** — buscador global arriba y tus **temas** (Python, Finanzas…) como tarjetas.
  Dentro de cada tema, tu avance en **unidades numeradas y en orden** — «1. Lo básico»,
  «2. Condicionales», «3. Bucles»… — con la actual marcada «◀ aquí voy». Cada unidad
  acumula sus notas; cuando avanzas, creas la siguiente unidad y sigues. El botón «+ Nota»
  pide dos cosas (título y qué aprendiste) y cae solo en la unidad donde estás.
- **🔁 Repasar** — la única función inteligente a la vista: cuántas notas vencen hoy y un botón
  para repasarlas. Cada nota tiene su propio calendario (repaso espaciado): si la recuerdas se
  aleja, si la fallas vuelve pronto. Al abrir la app, una pregunta del día de 15 segundos.
- **⚙️ Ajustes** — tema, áreas, estadísticas, respaldo.

Cada nota es una sola pantalla con tres preguntas:

1. **¿Qué aprendí?** — con tus palabras.
2. **El comando · la fórmula · el ejemplo** — en letra de código, con botón de copiar.
3. **¿Cómo lo practiqué?** — la evidencia de que lo hiciste de verdad.

Y un apartado **«Más»** plegado para lo que no siempre hace falta: campos extra (pasos,
errores, ejemplos…), conexiones entre notas, dudas, fuentes y el historial de correcciones.

### Enlaces `[[así]]`

Escribe `[[inventarios]]` dentro de cualquier campo. Si esa nota existe, queda enlazada; si no,
aparece en «Hoy» como concepto pendiente de crear. Es la forma de que nada se te quede fuera.

### Nivel de dominio

`Aprendiendo → Comprendido → Practicado → Aplicado → Dominado`. Filtra por «⚠️ Por dominar»
para ver qué tienes fresco y qué ya es tuyo de verdad.

### Historial de correcciones

Cuando descubras que entendías algo mal, regístralo en *Historial*: **antes pensaba X, ahora
entiendo Y**, con fecha. Es la prueba más honesta de aprendizaje real, y la nota no se
sobrescribe: la corrección queda guardada aparte.

## Instalar en el iPhone

1. Abre `https://<tu-usuario>.github.io/app-mis-finanzas/conocimiento/` en **Safari**.
2. **Compartir → Agregar a pantalla de inicio**.

Funciona sin internet y aparece como una app más.

> 💡 **Respalda de vez en cuando.** Tus notas viven solo en este dispositivo. Safari puede
> borrar los datos de sitios que no visitas en semanas. En **Ajustes → Respaldar (JSON)**
> descargas todo; guárdalo en iCloud. El export a **Markdown** te deja llevarte las notas a
> cualquier otra app.

## Estructura

```
index.html    ← la app completa (HTML + CSS + JS, sin dependencias)
manifest.json ← manifiesto PWA
sw.js         ← service worker (offline)
icons/        ← ícono de la red de conocimiento
```

## Privacidad

Puedes compartir el enlace con quien quieras: cada persona obtiene su propia app vacía.
Tus notas viven **solo en tu dispositivo** — la app no tiene servidor, no pide cuenta y no
hace ninguna llamada a internet, así que nadie más puede leerlas (ni siquiera el autor).
La otra cara de esa moneda: si pierdes el dispositivo sin respaldo, nadie puede recuperarlas
por ti. **Ajustes → Respaldar (JSON)**, con regularidad.

## Licencia

Código bajo [licencia MIT](../LICENSE).

