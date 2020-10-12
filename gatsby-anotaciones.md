# Gatsby Anotaciones


## Gatsby Pages

Es bueno tener la sigueinte arquitectura del proyecto:

Una carpeta:
  - public: aqui se queda todo el deploy and build de gatsby, puedes borrarla con ```gatsby clean````````` y volver a generlos.
  - src : aqui va todo el codigo, tiene una carpeta paginas, que es especial e importante en gatsby.
    - assets: imagenes, svgs
    - components: componentes de react
    - pages: va el codigo y es una carpeta muy especial e importante en gatsby. LAs paginas en gatsby se pueden crear
    dinamicamente o por el enrutamiento el filesystem. Puedo redireccionar a las paginas en gatsby creando un
    archivo `.js` y lo podemos llamar desde la url ejem: `https://localhost:8000/pagina.js`.
    - styles: son los estilos
    - templates: es parecida a pages pero sirve para paginacion
  - static : archivos staticos y html o css todo lo que importemos deberia ser de aqui

  > Nota: Si hay un archivo '.gitkeep' es para que git no borre una carpeta vacia.

  Las pages en gastby normalmente son componentes de React:

``````''' ` `` `` ```````````` 
import React from 'react'

export default function HomePage(){
return (
<div>
<p>Hola soy un home page.</p>
</div>
);
}
'''``
