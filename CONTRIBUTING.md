# Contribuyendo con Kitsunity
Kitsunity es planeada para ser un bot multifuncional con apoyo de la cominidad, sientete libre de enviar un pull si estas interesado en ayudar UwU.

## Understanding the code.
Aqui podras entender la estructura de Kitsunity, el codigo no esta aqui debido a que prevengo que roben mis ideas unu.

Estructura del archivo
```lua
Kitsunity
├── commands -- Comandos.
│   └── subdir -- En estos subfolders van todas las categorias y comandos de Kitsunity.
├── commands.beta -- Los comandos que voy creando, los pongo aqui antes de ponerlos en la otra carpeta.
│   └── maintenance -- Aqui los comandos que aun nesesitas ser reparados o poseen errores.
└── src -- Funciones.
    └── json -- Aqui van funciones generales.
    └── kitsunity.weebly.com -- Esta carpeta posee los recursos del sitio web de Kitsunity.
```

## Creando eventos

Estas funciones se añadiran mas adelante, por ahora esto no es nesesario, solo lo pongo para informacion

```js
const Event = require("../structures/Event.js");

class MyEvent extends Event {
  constructor(...args) {
    super(...args, {
      name: "eventName"
      enabled: true
    })
  }

  async run(...args) {}
}
```

## Commands.

Mas adelante pondre como hago mis comandos aqui.

## Comments

Recomiendo 100% hacer comentarios cuando hagas alguna modificacion, de esta forma sabre donde se edito el comando:

**Mal**
```js
const id = doStuff();
if(!id) return ctx.reply("Not found.");
const role = ctx.guild.roles.cache.get(id);
await role.delete();
```
**Bien**
```js
// Busca el rol.
const id = doStuff();
if(!id) return ctx.reply("Not found.");

// Consige el rol.
const role = ctx.guild.roles.cache.get(id);
// Y lo elimina.
await role.delete();
```
No es nesesario saber programar, ya que mi codigo es entendible por si mismo, lo unico es poseer el entorno de trabajo adecuado (No el block de notas xD), ademas, no es nesesaria la documentación para entender el lenguaje JavaScript, pero igual si quieres aprender estoy gustosa de enseñarte nwn.
