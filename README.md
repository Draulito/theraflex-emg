# TheraFlex EMG - versión web en la nube

Esta versión está pensada para subirse como página estática a GitHub Pages, Vercel o Netlify.

## Cómo usar
1. Abre la página desde Chrome o Microsoft Edge en un computador.
2. Conecta el Arduino/sensor por USB.
3. Haz clic en "Conectar sensor".
4. Selecciona el puerto serial del Arduino.
5. Calibra el sensor desde el menú del juego.

## Importante
- El juego vive en la nube, pero el sensor EMG/Arduino debe estar conectado físicamente al computador que lo va a usar.
- Web Serial requiere HTTPS. GitHub Pages, Vercel y Netlify ya publican con HTTPS.
- El baud rate configurado es 9600, igual que `Serial.begin(9600)`.
- Si el navegador no permite Web Serial, usa Chrome o Edge en PC. Safari/iPhone y Firefox pueden no funcionar con Web Serial.

## Subir a GitHub Pages
1. Crea un repositorio nuevo.
2. Sube este `index.html`.
3. En Settings > Pages, publica desde la rama `main`.
4. Te dará una URL tipo `https://usuario.github.io/repositorio/`.

## Subir a Vercel
1. Entra a Vercel e importa el repositorio.
2. Framework: Other / Static.
3. Deploy.
