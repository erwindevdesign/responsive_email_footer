<center> <h1 style="color:#f29100;font-family: monospace;">Responsive Email Footer</h1> </center>
<center> <h2 style="color:#697477;">Firma digital para pie de correo electrónico.</h2> </center>
<center> <img width='600' src='https://i.imgur.com/EeasGOP.png'></center>

<details><summary><h3 style="color:#697477">📋 Tabla de contenido</h3></summary>
<p>

1. [Sobre el proyecto](#id1.0)
2. [Uso](#id2.0)
3. [Contribución](#id3.0)
4. [Licencia](#id4.0)

</p>
</details>

<h3 style="color:#697477">📌 Sobre el proyecto </h3><a name='id1.0'></a>

<img align='right' width='290'  src='https://i.imgur.com/Od8ElaN.png'></a>

<p style="text-align:justify">Dentro de las herramientas existentes en posicionamiento de marca, la implementación de una firma digital personalizada dentro de la estructura de un correo y su uso recurrente en el ámbito profesional, empresarial, de negocios, académico y político permite trasladar los conceptos de branding al receptor del correo.</p>

<p style="text-align:justify">La firma digital nos permite <a style="color:#1D70B7 "> instrumentalizar</a> la comunicación de la marca dentro de los diferentes usos cotidianos que hacemos del correo electrónico, otorgando al usuario un referente de validez en su comunicación con el receptor del correo, del mismo modo esta herramienta permite su uso en marketing segmentado por usuario y su posición en los diferentes hitos del <a style="color:#1D70B7 ">journey</a> de compra utilizando metodologías de marketing.</p>

<h3 style="color:#697477">🧑‍💻 Uso</h3> <a name='id2.0'></a>

La construcción de la firma digital se realizará mediante la implementación del preprocesador `PUG` de `HTML` el cual permitirá modularizar y aportar a `HTML` de cualidades de lenguajes de programación. Para modificar el contenido del la firma digital haremos uso de las `variables`, `mixins`, `includes` y `extends` declaradas en el archivo `template.pug` que permitirán extender los componentes contenidos. La siguiente guía mostrará como modificar el código de la firma digital.

```md
:: Estructura de carpetas y archivos

Repository/
|
├── signing.html
├── README.md
└── templates/
|
├── head.pug
├── signing.pug
└── template.pug
```

1. Las imágenes contienen una dinámica de intercambio respondiendo a las dimensiones de la pantalla en la que se visualice, la imagen del usuario no deberá superar los `150x150px` y en una visualización mayor a `600px` la podremos modificar en la `Ln 23, Col 128` del archivo `signing.pug` detro de `./templates/`, al cambiar la url en la propiedad `background: url( ... );` del elemento `<img>` que lo contiene. La imagen que se visualice en dimensiones de pantalla menor a `600px` se modificaran en la `Ln 7, Col 1155` del archivo `head.pug` detro de `./templates/`, al cambiar la url en la propiedad `background: url( ... );` de la clase `.userimage{ ... }` que la contiene.

2. La imagen de la compañía no deberá superar los `140x75px` y se modificara en la `Ln 31, Col 54` del archivo `signing.pug` detro de `./templates/`, al cambiar el atributo `src=' ... '` del elemento `<img>` que la contiene.

3. Las variables contendrán los `datos` y `url's` de imágenes que se pueden modificar con base en la siguiente estructura:

```pug
-var user = ["first name","[space]last name ","[space]surname", "position", "working area", "company legal name"]

-var contact = ["phone number(s)","email", "web site","address" ]

-var icon = ["phone__icon","email__icon","web site__icon","address__icon" ]

-var social = ["social__icon_1","social__icon_2", "social__icon_3","social__icon_4"]

-var terms = ["short_terms_of_service"]
```

>

4. Una vez personalizado el contenido, compilaremos el archivo `HTML` ejecutando por consola la siguiente instrucción cada vez que el archivo cambie:

```sh
pug -w ./templates/signing.pug -o ./ -P
```

El archivo se creará en la raíz del repositorio con el nombre `signing.html` y se podrá incrustar como firma digital desde diversos gestores de correo electrónico multiplataforma que permiten adjuntar una firma desde un archivo `HTML`.

<h3 style="color:#697477">🧮 Contribución</h3><a name='id3.0'></a>

Si tiene una sugerencia que mejoraría esto, `forkea` el repositorio y cree una solicitud de extracción. Cualquier contribución que hagas es muy apreciada.

1. `Fork` al proyecto

2. Cree una rama `feature` (`git checkout -b feature/NewFeature`)

3. Confirme sus cambios (`git commit -m 'Hola! agregue una nueva característica'`)

4. `Push` a la rama (`git push origin feature/NewFeature`)

5. Abrir un `Pull Request`.

<h3 style="color:#697477">📜 Licencia</h3><a name='id4.0'></a>

Construido bajo la licencia MIT. Consulte <a href="../LICENSE" > LICENSE</a> para obtener más información.

<br>

<p align="center">
<img src="https://img.shields.io/badge/STATUS-EN%20DESAROLLO-green">
<img src="https://img.shields.io/badge/license-MIT-green">
</p>

---

<h3 style="color:#697477;text-align:center;">⚒️ Construido con</h3>
<p align='center'>
<img src='https://img.shields.io/badge/html-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white'>
<img src='https://img.shields.io/badge/Pug-FFF?style=for-the-badge&logo=pug&logoColor=A86454'>
<img src='https://img.shields.io/badge/css-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white'>
<img src='https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white'>
<img src='https://img.shields.io/badge/adobe%20illustrator-%23FF9A00.svg?style=for-the-badge&logo=adobe%20illustrator&logoColor=white'>

<!--

Las diferencias de interpretación de código entre los gestores de correo electrónico, las diferencias de visualización entre motores de renderizado en los diversos navegadores y las diferentes dimensiones de visualización en los dispositivos donde visualizaremos el correo electrónico crean la necesidad de desarrollar la estructura en código del producto bajo características de desarrollo que se integren y adecuen a estos requerimientos sin afectar la calidad del producto final. Para ello definir los siguientes atributos e implementar las siguientes características en la escritura del código ayudará a integrar estas diferencias de interpretación del código y minimizar las discrepancias de visualización.


 -->

<p style="color:'red';"  align='center'; > </br> </br> Your feedback 💚 is always appreciated!
</br> @erwindevdesign
 
 </a>&nbsp;&nbsp;


</p>
