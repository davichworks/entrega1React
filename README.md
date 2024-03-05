# Entrega1 React

## Gestión de Rutas

La gestión de rutas en esta aplicación se realiza utilizando la biblioteca React Router. A continuación, se detalla cómo se gestionan:

<h4>Definición de Rutas:</h4> Se importan los componentes Routes, Route y Link de React Router. Las rutas se definen dentro del componente <Routes>, donde cada ruta está asociada a un componente específico que se renderizará cuando la URL coincida con la ruta especificada.

![image](https://github.com/davichworks/entrega1React/assets/70800903/a6393155-6548-4812-affd-d3d6c627beeb)

<h4>Navegación entre Rutas:</h4> En la barra de navegación (<nav>), se utilizan los componentes Link de React Router para crear enlaces a las diferentes rutas de la aplicación. Estos enlaces permiten a los usuarios navegar entre las páginas de la aplicación sin necesidad de recargar la página completa.

![image](https://github.com/davichworks/entrega1React/assets/70800903/d102ab5e-573a-4088-89ac-3f8b8846ac77)

<h4>Rutas Protegidas:</h4> Algunas rutas, como "/admin" y "/mod", están protegidas y solo son accesibles para usuarios autenticados con roles específicos. Esto se maneja condicionalmente en la barra de navegación, donde se muestran los enlaces correspondientes solo si el usuario tiene los roles adecuados.

![image](https://github.com/davichworks/entrega1React/assets/70800903/99d87078-089a-42a0-9bd1-6b01a93d2b65)

## Gestión del Estado
La gestión del estado en esta aplicación se realiza utilizando el componente de clase App y el método setState. A continuación, se detalla cómo se maneja el estado:

<h4>Inicialización del Estado:</h4> En el constructor de la clase App, se inicializa el estado de la aplicación con valores predeterminados, incluyendo banderas booleanas para determinar si se deben mostrar ciertos tableros y el usuario actual.

![image](https://github.com/davichworks/entrega1React/assets/70800903/fb013047-5cfd-4d24-ba06-c1b8be2dc406)

<h4>Actualización del Estado al Montar el Componente:</h4> En el método componentDidMount, se obtiene el usuario actual y se actualiza el estado en consecuencia, determinando si el usuario tiene roles de moderador,administrador o ninguno.

![image](https://github.com/davichworks/entrega1React/assets/70800903/317359a4-8442-4ee5-973f-bb9813270bc3)

<h4>Cerrar Sesión y Actualización del Estado:</h4> El método logOut se llama cuando se hace clic en el enlace de "LogOut". Este método cierra la sesión del usuario y restablece el estado de la aplicación eliminando la información del usuario actual y estableciendo las banderas de roles en false.

![image](https://github.com/davichworks/entrega1React/assets/70800903/3af1edf3-41ef-4554-aa7e-3b634935a3c1)

