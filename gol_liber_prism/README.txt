GOL DEL LIBER - PRISM Live

Archivos:
- public/control.html: botonera del Android
- public/overlay.html: fuente web para PRISM en iPhone
- public/gol.webm: animacion original de OBS
- server.js: servidor WebSocket para sincronizar los celulares

PARA PUBLICAR
1. Subi el contenido de esta carpeta a un repositorio privado de GitHub.
2. Crea un servicio Web en un hosting Node.js compatible con WebSockets y HTTPS (por ejemplo Render).
3. Build command: npm install
4. Start command: npm start
5. Configura la variable de entorno CONTROL_TOKEN con una clave larga privada.
6. El hosting te entregara una direccion HTTPS, por ejemplo https://tu-servicio.onrender.com

ANDROID: abrir https://tu-servicio.onrender.com/control, escribir la clave y tocar el boton.
iPHONE: agregar https://tu-servicio.onrender.com/overlay como fuente web de PRISM, por encima de la camara.

LIMITACIONES IMPORTANTES
- PRISM Live en iOS debe permitir ejecutar WebSockets, reproducir WebM VP9 con alfa y audio y mantener transparente la fuente web. No esta garantizado: comprobar antes de usar en vivo.
- En iOS la reproduccion de audio iniciada remotamente puede bloquearse por la politica de autoplay. Si pasa, el festejo podria mostrarse sin audio o no reproducirse.
- Algunos hostings gratuitos suspenden servicios inactivos y la primera conexion puede tardar.
- No incluye automaticamente el marcador KeepTheScore; se conserva su fuente web actual.
- No hay URL publica operativa hasta que publiques el servicio.
