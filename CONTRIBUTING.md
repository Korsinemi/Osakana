# Contribuyendo con Osakana
Kitsunity es planeada para ser un bot multifuncional con apoyo de la cominidad, sientete libre de enviar un pull si estas interesado en ayudar UwU.

## Entendiendo el codigo
Aqui podras entender la estructura de Kitsunity, el codigo no esta aqui debido a que prevengo que roben mis ideas unu.


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

## Comandos

Mas adelante pondre como hago mis comandos aqui.

## Commentarios

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
