# crisol-remote-config

Config remota de Crisol. `RemoteConfig` (autoload del juego) lee
`config.json` de este repo vía `raw.githubusercontent.com` al arrancar. Si
la petición falla o tarda más de 4s, el juego se queda con sus valores por
defecto — nunca bloquea el arranque.

Repo público a propósito: separado del código fuente del juego (privado),
para no tener que exponerlo solo por esto. No contiene nada sensible, solo
flags de encendido/apagado de anuncios.

Editar `config.json` y hacer push alcanza para cambiar el comportamiento en
producción sin publicar una nueva versión — es el interruptor de
emergencia remoto (ver CLAUDE.md del repo de Crisol, y el comentario en
`autoloads/remote_config.gd`).
