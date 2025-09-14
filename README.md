Resolucion de preguntas

1. ¿Por qué aprender CSS avanzado?

Aprender CSS avanzado es fundamental por varias razones clave que impactan directamente en la calidad y profesionalismo de un sitio web:

- Mejora la experiencia de usuario (UX): Permite crear interfaces más atractivas, interactivas y fáciles de usar mediante animaciones, transiciones y layouts complejos.
- Diseño adaptativo (Responsive Design): Asegura que el sitio web se vea y funcione correctamente en cualquier dispositivo, desde teléfonos móviles hasta computadoras de escritorio.
- Mayor control y especificidad: Otorga un control preciso sobre el estilo de cada elemento, permitiendo diseños detallados y consistentes.
- Desarrollo profesional: Estas habilidades son muy demandadas en el mercado laboral actual, ya que son la base para crear sitios web modernos y competitivos.
- Eficiencia y mantenibilidad: El uso de herramientas como Flexbox, Grid y Variables CSS hace que el código sea más escalable, fácil de mantener y más rápido de escribir.

2. ¿Por qué cambia el posicionamiento de las cajas internas al div principal?
   
El posicionamiento de las cajas internas cambia porque la propiedad flex-direction define la dirección del eje principal del contenedor flex.
Por defecto, el eje principal es horizontal (flex-direction: row). Esto hace que los elementos se alineen uno al lado del otro.
Al cambiar la propiedad a flex-direction: column, el eje principal se vuelve vertical. Como los elementos flex siempre se alinean a lo largo del eje principal, ahora se apilan uno debajo del otro.

3. ¿Se puede lograr un cambio en el orden de los elementos sin tocar los archivos HTML, solo a través de CSS?
 
Sí, absolutamente. Esta es una de las mayores ventajas de los módulos modernos de CSS como Flexbox y Grid.
Con Flexbox: Se puede utilizar la propiedad order en los elementos hijos. Por defecto, todos los elementos tienen un order: 0. Al asignarles números diferentes (positivos o negativos), podemos cambiar su orden visual sin alterar el HTML.
Con Grid: Es aún más potente. La propiedad grid-template-areas permite crear un mapa visual del layout. El orden de los elementos en el HTML es irrelevante; lo único que importa es a qué "área" del grid se asigna cada elemento en el CSS.

4. ¿Qué hacen las propiedades width en el ejemplo de Flexbox?

En ese ejemplo, las propiedades width trabajan en conjunto con flex-wrap: wrap para crear un layout responsivo básico:
width: 33% se aplica a todos los div hijos. Intenta que cada caja ocupe un tercio del ancho del contenedor.
width: 64% se aplica específicamente al primer hijo (:first-child), sobrescribiendo la regla anterior y haciendo que ocupe aproximadamente dos tercios del ancho.
El resultado es que el primer elemento (64%) y el segundo (33%) suman un 97%, por lo que caben en la primera fila. El tercer elemento (33%) ya no cabe en esa fila, y gracias a flex-wrap: wrap, "salta" a la siguiente línea.

5. ¿Puedo diseñar toda mi web usando GRID?

Sí. De hecho, CSS Grid fue creado específicamente para ese propósito. Es la herramienta más poderosa y adecuada para diseñar la maquetación o el layout principal de una página web (la estructura de dos dimensiones que incluye header, footer, sidebar, contenido principal, etc.).
Mientras que Flexbox es excelente para alinear elementos en una sola dimensión (una fila o una columna), Grid maneja ambas dimensiones a la vez, dándote un control total sobre la estructura completa de la página.

6. ¿Por qué se dan estos cambios de layout con tan pocas líneas de diseño CSS usando Grid?

La eficiencia de CSS Grid se debe a su naturaleza declarativa. En lugar de dar instrucciones paso a paso sobre cómo posicionar cada elemento (usando floats, márgenes, etc.), con Grid simplemente declaramos cómo queremos que se vea el resultado final.
La propiedad grid-template-areas es el mejor ejemplo de esto: dibujamos un "mapa" del layout con texto. El motor de CSS se encarga de todo el trabajo complejo de calcular tamaños y posiciones para que los elementos encajen en ese mapa. Esto resulta en un código mucho más limpio, legible y potente con muchas menos líneas.                                      
