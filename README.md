# ClanCAPEL
Clan Capel, comunidad Valdiviana

## Publicar la página

El workflow de GitHub Actions habilita GitHub Pages y publica `index.html` cada vez que hay cambios en `main`. La página estará en:

https://markbuffalo1.github.io/ClanCAPEL/

## Compartir cambios con Firebase

Sin configurar Firebase, las fichas y el plan se guardan solo en el dispositivo de cada visitante. Para compartirlos:

1. Crea una Realtime Database en Firebase.
2. Copia `database.rules.json` en las reglas de esa base de datos y publícalas.
3. En `index.html`, pega la URL de la base de datos en `DB_URL`, sin `/` al final.
4. Publica esos cambios en `main`.

La ruta compartida es `/capel/public`. Sus reglas permiten lectura y escritura anónimas: cualquier persona con acceso a la página o a la base puede leer, modificar y borrar esos datos. No uses esta configuración para información privada ni pongas enlaces privados de Discord. Para restringir quién edita, reemplaza las reglas por autenticación antes de conectar la base.
