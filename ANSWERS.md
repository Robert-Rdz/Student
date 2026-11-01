# Respuestas — Profile Card

## 1. ¿Cuál es el valor por defecto de `flexDirection` en React Native? ¿En qué se diferencia de CSS en la web?

En React Native es column, así que los elementos se acomodan de arriba hacia abajo. En CSS para web el valor por defecto es row, de izquierda a derecha.

## 2. ¿Cuál es la diferencia entre `justifyContent` y `alignItems`?

justifyContent acomoda los elementos en la dirección principal (la que marca flexDirection) y alignItems en la dirección contraria. En una columna, justifyContent los mueve arriba y abajo, y alignItems a los lados.

## 3. ¿Qué hace `flex: 1` dentro de una fila? ¿Y en el `View` más externo de la pantalla?

En una fila, flex: 1 hace que el elemento ocupe el espacio que sobra, y si varios lo tienen se lo reparten por igual. En el View más externo hace que ocupe toda la pantalla.

## 4. ¿Cuál es la diferencia entre `resizeMode="cover"` y `resizeMode="contain"`?

cover hace que la imagen llene todo el espacio aunque se recorte una parte. contain muestra la imagen completa aunque queden espacios vacíos.

## 5. ¿Por qué usamos `StyleSheet.create` en lugar de objetos simples dentro del JSX?

Porque los estilos se crean una sola vez fuera del componente y no en cada render. Además, el código queda más ordenado y fácil de leer.

## 6. ¿Por qué una sombra escrita con `shadowColor` no aparece en Android?

Porque las propiedades shadow son de iOS y Android no las usa para dibujar sombras. En Android la sombra se hace con elevation.
