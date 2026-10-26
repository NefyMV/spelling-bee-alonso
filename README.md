# Spelling Bee de Alonso — primera versión

## Contenido
- `index.html`: aplicación web adaptable a celular y computadora.
- `words.json`: catálogo de palabras y referencias al audio.
- `audios/`: 42 audios originales suministrados.
- `README.md`: estas instrucciones.

## Publicar con GitHub Pages
1. Descarga y descomprime el ZIP.
2. Crea un repositorio en GitHub (por ejemplo, `spelling-bee-alonso`).
3. Sube `index.html`, `words.json`, la carpeta `audios/` y `README.md` a la raíz del repositorio. No subas solamente el ZIP.
4. En el repositorio abre **Settings → Pages**.
5. En **Build and deployment**, selecciona **Deploy from a branch**, la rama `main` y la carpeta `/ (root)`, y guarda.
6. Espera a que GitHub Pages publique la dirección.

## Modos incluidos
- Aprender: muestra palabra, página registrada, guía de deletreo y audio original.
- Practicar: oculta la palabra hasta revelar la respuesta y permite marcar si se sabía.
- Concurso: ronda aleatoria de 10 palabras, audio, respuesta oculta y evaluación manual por un adulto.
- Repasar errores: lista de palabras marcadas para practicar otra vez.

## Cómo agregar palabras después
1. Copia el nuevo MP3 a `audios/` con un nombre único, por ejemplo `audio43.mp3`.
2. Agrega un objeto al arreglo de `words.json` siguiendo esta estructura:
   {
     "audio": "audio43.mp3",
     "word": "example",
     "page": 43,
     "guide": "i - eks - ei - em - pi - el - i",
     "status": "pendiente de cotejo"
   }
3. Sube los cambios al repositorio. Usa la palabra y la guía de la tarjeta original; no las inventes.
4. Verifica que el nombre del archivo coincida exactamente con el campo `audio`.

## Importante
- Esta versión utiliza los 42 archivos de audio incluidos en el ZIP de origen.
- El concurso no escucha ni evalúa automáticamente la voz de Alonso. El adulto marca “Correcta” o “Incorrecta” después de escucharlo.
- El progreso se guarda en el almacenamiento local del navegador y dispositivo; no se sincroniza entre dispositivos.
- La guía se muestra tal como está en el Excel recibido. Conviene cotejarla con cada tarjeta antes de considerar la transcripción definitiva.
- Las imágenes/ilustraciones de las tarjetas no se incluyen en esta primera versión.
