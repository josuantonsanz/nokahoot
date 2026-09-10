# nokahoot

Juego de repaso de Religión para 1.º de ESO, pensado para proyectarse en clase y responder de forma conjunta.

## Uso

El proyecto no necesita instalación ni dependencias. Para ejecutarlo con un servidor local:

```bash
python3 -m http.server
```

Después, abre <http://localhost:8000> en el navegador.

> No conviene abrir `index.html` directamente con doble clic, porque algunos navegadores bloquean la lectura de `preguntas.json` desde archivos locales.

## Contenido

- `index.html`: interfaz y lógica del cuestionario.
- `preguntas.json`: presentación y banco de 30 preguntas, editable sin tocar el código.

## Personalizar preguntas

Cada pregunta de `preguntas.json` contiene:

- `category`: bloque temático mostrado en pantalla.
- `difficulty`: `facil` o `medio`.
- `question`: enunciado.
- `options`: dos opciones para verdadero/falso o cuatro para elección múltiple.
- `answer`: índice (empezando en 0) de la respuesta correcta.

El cuestionario permite comenzar las preguntas en orden o en orden aleatorio.
