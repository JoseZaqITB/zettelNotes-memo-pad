# Desarrollo web
## Diccionario
- **Hidratacion**: añadir un script a un html para hacerlo dinamico
- **Minificacion**: reducir el tamaño de los archivos
- **Transpileacion**: cambia tu codigo para hacerlo compatible con versiones de js antiguas
## Estrategias de Diseño Web
- **Single-page applications (SPA)**: un unico HTML, con un script para la interaccion con el usuario 
- **Static Side Generator (SSG)**: un HTML por pagina o URL, pero son pre-construidos y nunca cambian
- **Server-side Rendering (SSR)**: un html por pagina o URL, pero generado segun la solicitud del usuario
> Se pueden fucionar -> Se envia un html completo por cada pagina segun los datos que el usuario envie (SSR), pero aquel html usa js del cliente para la interactividad (SPA) 

> Existen meta-frameworks React especilizada en una arquitectura -> NEXTJS: hibrida, GATSBY: ssg, REACT: SPA 
## Herramientas
### Module bundler
Quieres hacer un projecto web que sea legible de aqui a 50 años? 
Pues usa module coding, te permite importar/exportar otros archivos de codigo a tu archivo de codigo con una linea. Asi podes independizar cada pagina/utilidad de los demas. 

Pero hay un problema. Si subis tal cantidad de pequeños archivos, tu pagina web va a ser muy lenta. 

Solucion?

Usa un empaquetador de modulos, la cual analiza tu codigo y minimiza todos tus archivos en uno ( bundle.js, index.css, index.html )
#### Ademas
Con plugins puedes: 
- aplicar los cambios en tiempo real para el desarrollo ( Hot Module replacement)
- Loaders: procesar archivos NO JS como: style-loader (css), file-loader (imgs, fonts)
#### Tops
- Webpack ( ya esta viejito, hay otras mejores)
- Vite 
- Parcel
- RollUp

## Frameworks
### REACT
Es una libreria que permite crear paginas web de manera dinamica usando JS.
#### Init
Se puede usar un initizialer de React para crear un projecto con la estructura y herramientas basicas para empezar a trabajar.
- **Create-react-app (CRA)**: las mas popular, usa webpack ( it is deprecated now)
- **Vite --template React**: enfoque en la velocidad
- **create-next-app**: app complejas, app hibridas ( SSG, SSR, CSR)
- **Parcel**: configuracion sencilla
- **Gatsby**: SSG 