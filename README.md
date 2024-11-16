# Chatty 

## Instrucciones para trabajar con submódulos en Git

## 1. Clonar el repositorio principal
El primer paso es clonar el repositorio principal como de costumbre:

```bash
git clone https://github.com/imdaviddev/Chatty.git
cd Chatty
```

---

## 2. Inicializar y actualizar los submódulos
Una vez dentro del repositorio principal, el colaborador debe inicializar y actualizar los submódulos para descargarlos correctamente:

```bash
git submodule init
git submodule update
```

Este comando descargará el contenido de los submódulos en las carpetas correspondientes.

---

## 3. Clonar con submódulos en un solo paso (opcional)
Para evitar el paso de inicializar y actualizar los submódulos manualmente, se puede usar el siguiente comando al momento de clonar:

```bash
git clone --recurse-submodules https://github.com/imdaviddev/Chatty.git
```

Esto clona el repositorio principal **y** los submódulos en un solo paso.

---

## 4. Mantener los submódulos actualizados
Si los submódulos se actualizan en el repositorio principal (por ejemplo, al cambiar la referencia del commit en el submódulo), el colaborador debe actualizar los submódulos localmente:

```bash
git submodule update --remote
```

---

## Archivos importantes a revisar
- **`.gitmodules`:** Este archivo contiene la configuración de los submódulos (URL y ruta).
- **`.git/config`:** Aquí se almacenan las referencias locales a los submódulos.

---

## Resumen para el colaborador

### Clonar el repositorio principal:

```bash
git clone --recurse-submodules https://github.com/imdaviddev/Chatty.git
```

### O, si ya se clonó:

```bash
git submodule init
git submodule update
```

Con esto, el proyecto estará listo con los submódulos correctamente configurados. 🎉
