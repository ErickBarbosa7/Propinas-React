# Calculadora de Propinas y Consumo
![Vista del Proyecto](./assets/image.png)

## Tecnologías Utilizadas

* **React (v18):**
* **Vite:**
* **Tailwind CSS**
* **JavaScript**

## Conceptos de React Aplicados

* **Componentes:** Separación de la interfaz en piezas reutilizables (`Header`, `Menu`, `Consumo`).
* **State (Estado):** Uso del hook `useState` para manejar dinámicamente el carrito de compras (`order`) y el porcentaje de propina seleccionado (`tip`).
* **Props:** Comunicación entre componentes, pasando datos (como el menú) y funciones (como `addItem` o `removeItem`) del componente padre (`App`) a los hijos.
* **Renderizado de Listas:** Uso del método `.map()` de JavaScript junto con la propiedad `key` para iterar sobre la base de datos y renderizar el menú y el resumen de la orden dinámicamente.
* **Interpolación:** Inserción de variables y ejecución de operaciones matemáticas directamente en la interfaz usando llaves `{}`.
* **Eventos:** Manejo de interacciones del usuario mediante `onClick` y `onChange`.
* **`.findIndex()`:** Utilizado para buscar si un platillo ya existe en la orden antes de agregarlo. Si existe, se actualiza la cantidad sin duplicar el registro; si no, se agrega como un elemento nuevo.
* **`.filter()`:** Utilizado en la función de eliminar elementos de la orden, creando un nuevo arreglo que excluye el ID seleccionado.
* **Inmutabilidad:** Al actualizar el estado, se utilizaron copias de los arreglos (Spread Operator `...`) para evitar mutar el estado original directamente, siguiendo las mejores prácticas de React.
