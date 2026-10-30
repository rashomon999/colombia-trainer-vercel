# Colombia Trainer — Landing (redirección a Google Play)

Página estática (solo español, como la app) para poner en la bio de Instagram. Enlaza a:
https://play.google.com/store/apps/details?id=com.colombia.trainer

## Desplegar en Vercel
`npx vercel --prod` desde esta carpeta → "Create a new project" → nombre `colombia-trainer`.
Sin build: todo es estático.

## Cambiar el link de Google Play
La constante `PLAY_URL` en el `<script>` del final de `index.html`.

## iPhone
La app es solo Android: si la página se abre en un iPhone, aparece un aviso bajo el botón.

## Capturas
`img/*.jpg` salen de `ColombiaTrainer/play/captura_*.png`. Si cambias las capturas,
reemplaza los archivos con el mismo nombre.

## Redirección automática
`AUTO_REDIRECT = true` hace que la página salte sola a Google Play tras `AUTO_REDIRECT_DELAY` ms
(nunca en iPhone).
