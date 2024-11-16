# Chatty un sistema de chat 

## Clonar el proyecto con submódulos

Este proyecto utiliza **submódulos de Git** para gestionar repositorios externos. 
Sigue estos pasos para clonar el repositorio correctamente:

### Clonar el repositorio principal

1. Clona el repositorio principal:
```bash
git clone --recurse-submodules https://github.com/imdaviddev/Chatty.git
``` 

2. El parámetro --recurse-submodules asegura que los submódulos se clonen automáticamente.
  Accede al directorio del proyecto:
```
cd Chatty
```

## Si olvidaste clonar con --recurse-submodules. Si ya clonaste el repositorio principal sin 
   incluir los submódulos, inicialízalos y actualízalos manualmente:

1. Inicializa los submódulos:
```
git submodule init
```

2. Descarga el contenido de los submódulos:
```
git submodule update
```

## Mantener los submódulos actualizados
Si los submódulos cambian en el repositorio principal (por ejemplo, al actualizar un commit en un submódulo), ejecuta el siguiente comando para sincronizar los cambios:

```
git submodule update --remote
```

Con estos pasos, tu entorno estará correctamente configurado para trabajar con este proyecto. 🚀
