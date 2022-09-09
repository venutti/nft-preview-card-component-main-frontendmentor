# Frontend Mentor - NFT preview card component

Esta es una solución al [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Los desafíos de Frontend Mentor ayudan a mejorar las skills al codear construyendo proyectos realistas.

## Tabla de Contenidos

- [Resumen](#resumen)
  - [El desafío](#el-desafío)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [Mi proceso](#mi-proceso)
  - [Construido con](#construido-con)
  - [Lo que aprendí](#lo-que-aprendí)
  - [Desarrollo continuo](#desarrollo-continuo)

## Resumen

### El desafío

Los usuarios deberían poder:

- Ver el layout más óptimo, independientemente de la pantalla de su dispositivo
- Ver 'hover states' para elementos interactivos

### Screenshot

![Captura desde 2022-09-08 23-26-15](https://user-images.githubusercontent.com/87911089/189262720-9aead77e-7245-4f14-8519-e81093d076c1.png)


### Links

- Solution URL: [GitHub](https://github.com/venutti/nft-preview-card-component-main-frontendmentor)
- Live Site URL: [GitHub Pages](https://your-live-site-url.com)

## Mi proceso

### Construido con

- Etiquetas HTML5 semánticas
- Variables de CSS
- Flexbox
- Desarrollo Mobile-first


### Lo que aprendí

Una de las estrategías más útiles que aprendí fue la de agregar un 'filtro' delante de una imagen al hacer *hover*:

![Captura desde 2022-09-08 23-27-17](https://user-images.githubusercontent.com/87911089/189262770-ae7ce1c4-dd49-4431-8249-4dec36b18f1c.png)

Para ello, usé lo siguiente:

```html
<div class="img">
  <img src="./images/image-equilibrium.jpg">
  <div class="eye"><img src="./images/icon-view.svg"></div>
</div>
```
```css
.card .img {
    position: relative;
    cursor: pointer;
}
.card .img .eye {
    position: absolute;
    width: 100%;
    height: 100%;
    background-color: var(--CYAN);
    top: 0;
    opacity: 0;
}
.card .img .eye:hover {
    opacity: .5;
}
```
También es importante remarcar que las imágenes y los inputs **no pueden tener pseudo elementos ::before y ::after**. Para mayor información, consultar este [link](https://stackoverflow.com/questions/6949148/css-after-not-adding-content-to-certain-elements/6949190#6949190).


### Desarrollo continuo

Reveer el concepto de entregar un *componente*, y de ampliar el uso de texto y espaciado *responsive*.
