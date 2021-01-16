# Flexbox
- Es un diseño de layout.
- Necesita de un contenedor padre e hijo para funcionar.
- Al agregar display flex al padre convierte en caja flexible a sus hijo no a padre.
## Manejo del main axis y cross axis
### Flex direction row
- Main axis »  justify-content » Width » Horizontal
  - Derecha hacia izquierda main start y main end ││ En modo inverso al colocar row-reverse
- Cross axis »  align-items » Heigth » Vertical
  - Arriba hacia abajo cross start y cross end ││ En modo inverso al colocar column-reverse
### Flex direction column
- Main axis »  justify-content » Heigth » Vertical
- Cross axis »  align-items » Heigth » Horizontal
## Propiedades del contenedor (padre)
- Align-items: flex-start │ flex-end │ center │ stretch │ baseline;
  - stretch: Usa todo el espacio que hay en el contenedor padre, dependiendo la direccion del eje principal sera el width o el heigth, /* Los elementos no deben tener width o heigth segun sea el caso */
  - baseline: Toma la line base del texto para poder alinearlos no importa el tamaño que tenga toma la linea del texto para alinearlo.
- Justify-content: flex-start │ flex-end │ center │ space-between │ space-around │ space-evenly;
  - space-between: Reparte el espacio que hay en el contenedor padre al centro.
  - space-around: Reparte el espacio entre ellos es como colocar un margin.
- Flex-wrap: nowrap │ wrap │ wrap-reverse;
  - wrap: indica si los elementos podran desplazarce o no en otro fila o columna (dependiendo la direccion del main axis).
- Flex-direction: row │ row-reverse │ column │ column-reverse;
  - Cambia el eje principal (main axis).
- Flex-flox: direccion │ wrap
  - Esta propiedad es un shorthand que incluye la direccion y el wrap en los items hijos.
## Propiedades del contenedor (hijo)
- aligh-self: flex-start │ flex-end │ center │ stretch │ baseline;
  - Usa los mismo atributos que align-items pero sobreescribe el atributo del item hijo.  
