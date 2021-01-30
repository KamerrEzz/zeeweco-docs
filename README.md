![Zeew Api](https://i.imgur.com/MP2bABn.png "Lo Mejor de Zeew y del C&P")

# Zeew Eco!
  - Economía Fácil y sencilla!
  - Tienda fácil de crear e intuitiva!

¡Crea una economía fácil y sencilla de usar para tu bot, ahora con ZeewEco!
¡Lo unico que necesitas en una base de datos de MongoDB (mas adelante te explicare el porque...)

## Informacion
* **Constructores**
  * [Economía](#economia)
  * [Tienda](#tienda)
  * [Dinero](#dinero)
  * [Inventario](#Inventario)
* **Estructura json**
  * [Economía](#json-eco)
  * [Tienda](#json-td)
* **Zeew**
  * [Staff](#staff)
  * [Proyectos](#proyectos)

No olvides que si tienes un error o propuesta para mejorar este NPM, solo tienes que unirte a este servidor de [Discord](https://discord.gg/HWwBD6F).

¡Gracias por confiar en nosotros!
## Instalación
```js
npm i zeew-eco
```

### Economia
```js
const zeeweconomy = require('zeew-eco')
const eco = new zeeweconomy.Economia()
```

| Métodos | Descripción |
| ------ | ------ |
| [ver](#Eco-ver) | Muestra el dinero del usuario
| [agregar](#Eco-agregar) | Agrega dinero aun usuario|
| [quitar](#Eco-quitar) | Elimina el dinero de un usuario|
| [reiniciar](#Eco-comprar) | Comprar En la tienda|
| [trabajar](#Eco-comprar) | Ganar una cantidad de dinero RANDOM|

#### Economia: Ver
```js
eco.ver(id, clave)
```
* id - ID del usuario
* clave - ID del servidor
```js
const eco = new zeco.economia()
eco.ver(miembro.id, servidor.id)
```
Retorno (Number)
```js
123123
```

#### Economia: Agregar
```js
eco.agregar(id, clave, cantidad)
```
* id - ID del usuario
* clave - ID del servidor
* cantidad - Dinero que quieras agregarle

```js
const eco = new zeco.economia()
eco.agregar(miembro.id, servidor.id, 1500)
```

#### Economia: Quitar
```js
eco.quitar(id, clave, cantidad)
```
* id - ID del usuario
* clave - ID del servidor
* cantidad - Dinero que quieras agregarle

```js
const eco = new zeco.economia()
eco.quitar(miembro.id, servidor.id, 1500)
```
#### Economia: Reiniciar
```js
eco.reiniciar(id, clave)
```
* id - ID del usuario
* clave - ID del servidor
* 
```js
const eco = new zeco.economia()
eco.trabajar(miembro.id, servidor.id)
```
#### Economia: Trabajar
```js
eco.trabajar(id, clave, cantidad)
```
* id - ID del usuario
* clave - ID del servidor
* cantidad - Cantidad maxima aleatoria

```js
const eco = new zeco.economia()
eco.trabajar(miembro.id, servidor.id, 1500)
```

### Tienda

```js
const zeeweconomy = require('zeew-eco')
const tienda = new zeeweconomy.Tienda()
```

| Metodos | Descripcion |
| ------ | ------ |
| [Mostrar](#TD-mostrar) | Muestra Items a la tienda|
| [Agregar](#TD-agregar) | Agrega Items a la tienda|
| [Eliminar](#TD-quitar) | Elimina Items de la tienda|


#### Tienda: Mostrar

```js
eco.mostrar(clave)
```
* clave - ID del servidor
```js
const td = new zeco.tienda()
eco.mostrar(servidor.id)
```
```js
```
<a name="TD-agregar" />

#### Tienda: Agregar

```js
eco.agregar(clave, nombre, desc, precio)
```
* clave - ID del servidor
* nombre - Nombre del Item
* desc - La descripcion del item
* precio - el precio del item
```js
const td = new zeco.tienda()
td.agregar(servidor.id, "Canal Propio", "un canal privado para ti", 20000)
```
```js
```
<a name="TD-quitar" />

#### Tienda: Eliminar

```js
td.eliminar(clave, item)
```
* clave -ID del servidor
* item - Numero del Item de la tienda
```js
const td = new zeco.tienda()
td.eliminar(servidor.id, 1)
```
```js
```
#### Tienda: Comprar

```js
eco.comprar(clave, id, item)
```
* clave - ID del servidor
* id - ID del usuario
* item - numero de item
```js
const eco = new zeco.economia()
eco.comprar(servidor.id, miembro.id, 1)
```
```js
```


### Inventario
```js
const zeeweconomy = require('zeew-eco')
const inventario = new zeeweconomy.Inventario()
```
| Metodos | Descripcion |
| ------ | ------ |
| [compras](#V-compras) | Guardar Compras en el inventario|
| [quitarcompras](#V-quitarcompras) | Quitar Alguna compra en el inventario |
| [vercompras](#v-vercompras) | Ver los objetos comprados desde la tienda


#### Inventario: compras
```js
inv.compras(clave, id, item, boleano)
```
* clave - ID del servidor
* ID - ID del usuario
* Item - ID del item de la tienda que sera guardado en el inventario
* boleano
    * true - No guardar el mismo Item
    * false - Guardar el mismo Item
> proximas Actualizaciones se quiere hacer que los usuarios puedan vender los items de sus inventarios y tener una economia mas amplia.
```js
const inv = new zeco.inventario()
inv.quitarcompras(servidor.id, usuario.id, 2 , false)
```

#### Inventario: quitarcompras

```js
inv.quitarcompras(clave, id, item)
```
* clave - ID del servidor
* ID - ID del usuario
* Item - ID del item de la tienda que sera eliminado en el inventario
```js
const inv = new zeco.inventario()
inv.quitarcompras(servidor.id, usuario.id, 2)

#### Inventario: vercompras
```js
inv.vercompras(clave, id)
```
* clave - ID del servidor
* ID - ID del usuario
```js
let inv = new ze.inventario()
inv.vercompras(servidor.id,usuario.id)
```


#### ¡Staff de Zeew!
 * @KamerrOficial
  ```
    * ROL: Owner
    * ID Discord: 403695999941345280
    * Redes Sociales: @KamerrOficial
    * Portafolio: behance.net/kamerroficial
  ```
 * @LHCLYT  
```
  * ROL: Editor de README & Amigo
  * ID Discord: 478572042384572424
  * Proyecto: https://cactusfire.xyz
  * Discord: https://discord.gg/73AMGUZ
```

#### Proyectos de Zeew

| Proyecto | Descripción |
| --- | --- |
| [ZEEW](https://www.npmjs.com/package/zeew) | Descubre nuestra API Reset de Imágenes y manipulación

```js
```
#### Donaciones
* [Kamerr Ko-fi](https://ko-fi.com/kamerroficial) ❤️
* [PayPal](https://www.paypal.com/donate/?hosted_button_id=MAB5M68DJG5PQ&source=url) ❤️
