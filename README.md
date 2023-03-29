
<img src="src/assets/angular.png" width="50"/>
<b style='font-size: 50px'>Angular </b>

<br/>

## **String Interpolation**
Nos ayuda a pasar datos a renderizar a nuestro template o nuestra vista "{{ myFuntion() }}" un breve ejemplo del String Interpolation

<b style='color: green; font-size: 20px'>Nota: </b>
Las variables para ser accedidas por el String Interpolation deben ser de acceso publico para poder ser leidas en el Html.

<br/>

## **Property** <b style="color: green;">[ Binding ]</b>
Es la forma en la que podemos modificar atributos desde el controlador .ts hasta el template html por ejemplo un href de una imagen, el estado de un boton, etc.

<br/>

## **String Interpolation o Property Binding?**
**String Interpolation** nos sirve mucho para ingresar contenido donde necesitemos renderizarlo.
Mientras que le **Property Binding** es usado especificamente para propiedades

<br/>

## **Event Binding**
El Event Binding le permite escuchar y responder a las acciones del usuario, como pulsaciones de teclas, movimientos del mouse, clics y toques (Atributos HTML y propiedades DOM).

Para vincular un elemento html a un evento, debemos indicar el nombre del evento entre paréntesis a la izquierda de un signo igual y el nombre de una funcion entre comillas a la derecha, recuerda indicar que se trata de una funcion con los parentecis “nameFunction()” .

```
  <input (keydown.shift.t)="onKeydown($event)" />
  <button (click)="increaseAge()">Age ++</button>
```

## **Data** <b style="font-size: 20px; color: green"> [(Binding)] </b>

* Importante recalcar que para hacer uso de ngModel debemos importar el “FormModule” y habilitar el mismo en app.module.ts

* ngModel raliza un seguimiento del valor y el estado de validación de un control de formulario individual debido a las propiedades que hereda de FormControl es recomentado saber como funciona dicho proceso.

* Podemos personalizar las validaciones que deberia tener un campo o el mismo formulario

* Aqui utilizamos las variables de referencia (las que tienen el signo #) y debemos indicar que la variable debera tomar el valor del ngModel <<#nameInput=“ngModel”>>

* Se pueden realizar las validaciones que normalmente encontramos en html y con “pattern” podemos especificar una comprobacion como exprecion regular

* Podemos tener un flujo de datos unidireccional con [] o bidireccional con [( )]

* Acepta inputs
* Cuando se utiliza el ngModel sin la etiqueta **form** es necesario proporcionar un “nombre de atributo” de manera que el control pueda ser registrado en el formulario padre bajo ese nombre.

<br/>

<b style="font-size: 30px;">*ngIf</b>

Nos permite hacer un renderizado condicional o validar por medio de
logica dentro de un elemento html div,span,etc. Si este debe ser mostrado o no.

<br/>

<b style="font-size: 30px;">*ngFor</b>

El ngFor nos permite iterar arreglos y listarlos en los templates html. por otra parte para iterar objetos en angular la mejor forma de hacerlo es creando interfaces y dandole el tipo de estructura para obligar a el objeto a tener esta cantidad y tipos de datos para asi evitar problemas ya sea con otros desarrolladores o con el comportamiento de los datos.

<br/>

<b style="font-size: 30px;">*NgClass & NgStyle</b>

Estas son directivas que nos ayudan a adjuntar una cantidad considerable de estilos y clases para asi solucionarnos la vida 
