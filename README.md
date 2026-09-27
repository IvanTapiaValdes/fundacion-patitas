* Fundación Patitas

Proyecto final del curso de Desarrollo Web en Coderhouse. Fundación Patitas es un sitio informativo para una fundación de rescate y adopción de animales: muestra quiénes son, los perros y gatos que están esperando hogar y los que ya lo han encontrado, se indica cómo es el proceso para adoptar y las distintas formas de colaborar (difusión,ser voluntario, donaciones etc).

* Repositorio: https://github.com/IvanTapiaValdes/fundacion-patitas
* Deploy en Netlify: https://cozy-sunshine-f3f397.netlify.app/


* Con qué está hecho

- HTML5
- SCSS, compilado a styles/styles.css. Usa variables, mixins, extend, nesting y partials separados por carpetas.
- Bootstrap 5.3.8, cargado desde CDN (navbar, carrusel, cards, formularios)
- AOS para las animaciones al hacer scroll
- Google Fonts (Poppins)


* Estructura

```
index.html
scss/
  main.scss        
  utilities/        
  base/             
  layout/           
  components/       
styles/
  styles.css        
pages/
  adoptame.html
  colabora.html
  como-adoptar.html
  sobre-nosotros.html
assets/
  logos, fotos de las mascotas, etc.
```

* Si quieren editar los estilos:

Los estilos no se editan directo en styles.css, ese archivo se genera solo. Hay que modificar los .scss y después correr los siguientes comandos:

```
npm install -g sass
sass scss/main.scss styles/styles.css --style=expanded

```

* Qué tiene el sitio:

- Cards con hover para mostrar servicios, proyectos y la sección de sobre nosotros
- Dos carruseles, uno de gatos y otro de perros con fotos en 800x600
- Navbar de Bootstrap, responsive, con el menú hamburguesa funcionando bien en mobile
- Grillas que se acomodan solas según el tamaño de pantalla
- Footer con redes sociales, que en pantallas grandes se pone en fila y en mobile se centra


* Para verlo funcionar:

Se puede abrir index.html directo con doble clic, o usando la extensión Live Server de VS Code para poder visulizarla. No hace falta instalar nada más.


* Autor

- Iván Tapia Valdés
- Proyecto: Fundación Patitas